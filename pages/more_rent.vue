<template>
    <div>    
        <div class="home-container mt-1">
            
            <div class="">
                <div class="text-center">
                    <h1 class="header-h2">Properties for Rent</h1>
                </div>
                <!-- cards -->
                <div class="container">
                    <div class="row justify-content-end">
                        <input type="search" class="form-control" placeholder="Search by State" v-model="filterByLocation">
                    </div>
                    <div class="row mt-5"  v-if="rentItems.length > 0">
                <div class="col-sm-12 col-md-12 col-lg-4 mb-2" v-for="(info,index) in filterAll" :key="index">
                    <div class="card shadow rounded">
                        <img
                            :src="info.photo_main"
                            class="card-img-top"
                            alt="..."
                        />
                        <div class="card-body">
                            <span class="city">{{info.address}}, {{info.city}}, {{info.state}}</span>
                            <div class="d-flex justify-content-between">
                                <div class="title">{{info.title}}</div>
                                <div>
                                    <span class="price">&#8358;{{info.price}}</span>/plot
                                </div>
                            </div>
                             <div class="icons">
                                <ul>
                                    <li>
                                        <img src="/img/icon/icon_1.png" alt="" srcset="">
                                    </li>
                                    <li>
                                        <img src="/img/icon/icon_2.png" alt="" srcset="">
                                    </li>
                                    <li>
                                        <img src="/img/icon/icon_3.png" alt="" srcset="">
                                    </li>
                                    <li>
                                        <img src="/img/icon/icon_4.png" alt="" srcset="">
                                    </li>
                                </ul>
                            </div>
                            <p class="mt-1">
                               <ul>
                                   <li>
                                       {{info.bedrooms}} Bedroom(s)
                                   </li>
                                   <li>
                                      {{info.bathrooms}} Restroom(s)
                                   </li>
                               </ul>
                            </p>
                             <p class="mt-1">
                               <ul>
                                   <li>
                                      {{info.sqft}} Square Fts
                                   </li>
                                   <li style="margin-left : .7rem">
                                      CCTV Surveillance
                                   </li>
                               </ul>
                            </p>
                        </div>
                        <div class="card-footer" @click="displayInfo(info.id)">More Information</div>
                    </div>
                </div>
                    </div>
                     <div class="text-center mt-5" v-else>
                        <Loader />
                    </div>
                    <div class="text-center mt-5" v-if="rentItems.length">
                        <h6>No more Properties</h6>
                    </div>
                    <!-- button More -->
                </div>
            </div>
        </div>

        <div>
            <div class="container mt-5 mb-5">
                <div class="row">
                    <div class="col-sm-12 col-md-12 col-lg-6">
                        <carousel-property />
                    </div>
                    <div class="col-sm-12 col-md-12 col-lg-6">
                        <form-management />
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
            rentItems:{},
            filterByLocation : ""
        }
    },
    computed:{
        filterAll(){
            try{
                return this.rentItems.filter((post)=>{
                    return(
                        post.state.toLowerCase().match(this.filterByLocation.toLowerCase() || this.filterByLocation.toUpperCase())
                    )
                })
            }
            catch (error) {
                console.log(error);
            }
        }
    },
    mounted(){
        this.getRentItems()
    },
    methods:{
        getRentItems(){
        this.$axios.get("https://jayceeandjay.online/rents", {headers : {'Content-Type':'application/json'}}).then((res)=> {
               this.rentItems=res.data.results;
               console.log(this.rentItems)
         }) 
    },
        displayInfo(info){
        this.$router.push(`/rent/${info}`)
    }
}
};

</script>

<style scoped>
@font-face {
    font-family: sofiaPro;
    src: url("/font/sofiaProRegular.ttf");
}
* {
    font-family: sofiaPro;
}
.form-edit {
    padding: 1rem 0 0 0;
}
.form-head {
    font-style: normal;
    font-weight: bold;
    font-size: 28px;
    line-height: 28px;
    letter-spacing: 0.03em;
    text-transform: uppercase;
    color: #002817;
}
.header-h2{
    margin-left: auto;
    margin-right: auto;
    color: #08804b;
}
label {
    color: #002817;
    font-style: normal;
    font-weight: bold;
}
input {
    /* background: #eff0f7; */
    width: 30%;
    margin-right: 1rem;
}
textarea {
    background: #eff0f7;
    width: 70%;
}
.btn-send {
    background: #08804b;
    border-radius: 6px;
    text-align: center;
    color: #fff;
    width: 70%;
}
.grid {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr;
}
.btn-success {
    width: 75%;
    display: block;
    margin: auto;
    margin-top: 2.5rem;
    padding-top: 1rem;
    padding-bottom: 1rem;
    margin-bottom: 2.5rem;
    background-color: #08804b;
    font-size: 1.5rem;
}
.carousel {
    margin: auto;
    width: 90%;
    margin-bottom: 3rem;
}
.carousel-item {
    height: auto;
}
.carousel-indicators li {
    /* border-radius: 100%; */
    background-color: #08804b;
}
.carousel-indicators {
    bottom: -50px;
}
.carousel-caption {
    width: 100% !important;
    position: absolute;
    right: 15%;
    bottom: 0 !important;
    left: 0 !important;
    z-index: 10;
    padding: 20px !important;
    color: #fff;
    background: rgba(28, 28, 28, 0.36) !important;
    backdrop-filter: blur(8px) !important;
    text-align: left !important;
}
h5 {
    font-style: normal;
    font-weight: bold;
    font-size: 32px;
    line-height: 46px;
    /* identical to box height */
    letter-spacing: 0.02em;
    color: #ffffff;
}
.wrapper {
    background: white;
    height: 65vh;
    background-size: cover;
    background-position: center;
}
.wrapper-content {
    margin: auto;
    width: 90%;
    padding-top: 2rem;
}
.wrapper-content img {
    width: 3rem;
    margin-right: 0.8rem;
}
.wrapper-content-one h6 {
    font-size: 20px;
    color: #08804b;
    text-transform: uppercase;
}
.wrapper-content-one h2 {
    font-size: 40px;
    font-weight: bold;
}
.wrapper-content-two {
    text-align: right;
    padding-top: 1.5rem;
}
.wrapper-content-two-one {
    font-size: 40px;
    font-weight: bold;
}
.wrapper-content-two-two {
    font-size: 25px;
}

.header-title {
    font-style: normal;
    font-weight: bold;
    font-size: 38px;
    line-height: 38px;
    text-align: center;
    letter-spacing: 0.02em;
    color: #08804b;
    /* text-shadow: 4px 4px 7px rgba(0, 0, 0, 0.25); */
    /* backdrop-filter: blur(44px); */
    text-transform: uppercase;
}
.header-text {
    font: Sofia Pro Light;
    font-weight: normal;
    font-size: 24px;
    line-height: 35px;
    text-align: center;
    letter-spacing: 0.02em;
    color: #c9c9c9;
    margin-top: 0.2rem;
    margin-bottom: 0.5rem;
}
.button-edit {
    display: flex;
    text-align: center;
    justify-content: center;
    align-items: center;
    margin-top: 2rem;
}
.btn-buy {
    background: #08804b;
    border-radius: 4px 0px 0px 4px;
    color: #fff;
    padding-left: 3rem;
    padding-right: 3rem;
    margin-left: -5px;
}
.btn-rent {
    background: #ebf5f1;
    border-radius: 0px 4px 4px 0px;
    color: #08804b;
    padding-left: 3rem;
    padding-right: 3rem;
    position: relative;
}
.search-session {
    background: #fff;
    padding: 1rem;
    display: flex;
    justify-content: space-between;
    margin-top: 2rem;
    border: #ebf5f1 1px solid;
    border-radius: 10px;
}
::placeholder {
    font-style: normal;
    font-weight: normal;
    font-size: 12px;
    line-height: 22px;
    /* text-align: center; */
    letter-spacing: 0.06em;
    color: #afafaf;
    margin-right: 0.5rem;
}
select {
    outline: none;
    border: none;
    width: 100%;
    padding: 0.5rem;
    color: #afafaf;
}
.stroke {
    color: #c4c4c4;
    margin-top: 0.5rem;
}
option {
    font-style: normal;
    font-weight: normal;
    font-size: 15px;
    line-height: 22px;
    text-align: center;
    letter-spacing: 0.06em;
    color: #afafaf;
}
.btn-search {
    background: #08804b;
    border-radius: 8px;
    color: #fff;
    padding-right: 3rem;
    padding-left: 3rem;
    /* width: 100%; */
}
.angle-edit {
    color: #fff;
    text-align: center;
    font-size: 24px;
    margin-top: 3rem;
    cursor: pointer;
}
.line-on-mobile {
    display: none;
}

/* homesection */
.home-container {
    background: rgba(42, 0, 162, 0.03);
    padding: 1rem 0 3rem 0;
}
.style-container {
    margin: 3rem 5rem 0 8rem;
}
.header-home {
    font-style: normal;
    font-weight: bold;
    font-size: 26px;
    line-height: 37px;
    text-align: center;
    letter-spacing: 0.1em;
    color: #5e5c5c;
}
.border-line {
    margin: auto;
    width: 223px;
    height: 5px;
    background: #02be20;
}
.city {
    font-style: normal;
    font-weight: normal;
    font-size: 12px;
    line-height: 17px;
    text-align: center;
    letter-spacing: 0.02em;
    color: #000000;
}
.title {
    font-style: normal;
    font-weight: bold;
    font-size: 18px;
    line-height: 28px;
    letter-spacing: 0.02em;
    color: #000000;
    margin-top: 0.5rem;
}
.price {
    font-style: normal;
    font-weight: bold;
    font-size: 16px;
    line-height: 26px;
    text-align: right;
    letter-spacing: 0.02em;
    color: #000000;
}
.card-footer {
    background: #02be20 !important;
    color: #fff;
    text-align: center;
    font-weight: bold;
    font-size: 14px;
    line-height: 20px;
    letter-spacing: 1.8px;
    text-transform: uppercase;
    cursor: pointer;
}
ul {
    padding: 0;
    margin: 0;
}
ul li {
    list-style-type: none;
    text-decoration: none;
    display: inline;
    margin-right: 1rem;
    font-style: normal;
    font-weight: normal;
    font-size: 13px;
    line-height: 19px;
    letter-spacing: 0.75px;
    color: #535353;
}

.view-more {
    font-style: normal;
    font-weight: normal;
    font-size: 20px;
    line-height: 32px;
    text-align: right;
    letter-spacing: 0.02em;
    color: #02be20;
    text-decoration: underline;
    cursor: pointer;
    /* margin: 1rem 8rem 0 5rem; */
}
.icons {
    margin-top: 0.5rem;
}
.icons ul li {
    background: rgba(8, 128, 75, 0.08);
    border-radius: 38px;
    padding: 0.3rem;
}
/* @media screen and (max-width: 768px) {
    .style-container {
        margin: 1rem;
    }
    .card {
        width: 100%;
    }
    .top-down {
        margin-top: 0.5rem;
    }
    .view-more {
        margin: 1rem 1rem 1rem 5rem;
    }
} */

/* rentsection */
.style-container {
    margin: 3rem 5rem 3rem 8rem;
}
.header-home {
    font-style: normal;
    font-weight: bold;
    font-size: 26px;
    line-height: 37px;
    text-align: center;
    letter-spacing: 0.1em;
    color: #5e5c5c;
}
.border-line {
    margin: auto;
    width: 80px;
    height: 5px;
    background: #02be20;
}
.city {
    font-style: normal;
    font-weight: normal;
    font-size: 12px;
    line-height: 17px;
    text-align: center;
    letter-spacing: 0.02em;
    color: #000000;
}
.title {
    font-style: normal;
    font-weight: bold;
    font-size: 18px;
    line-height: 28px;
    letter-spacing: 0.02em;
    color: #000000;
    margin-top: 0.5rem;
}
.price {
    font-style: normal;
    font-weight: bold;
    font-size: 16px;
    line-height: 26px;
    text-align: right;
    letter-spacing: 0.02em;
    color: #000000;
}
.card-footer {
    background: #02be20 !important;
    color: #fff;
    text-align: center;
    font-weight: bold;
    font-size: 14px;
    line-height: 20px;
    letter-spacing: 1.8px;
    text-transform: uppercase;
    cursor: pointer;
}
ul {
    padding: 0;
    margin: 0;
}
ul li {
    list-style-type: none;
    text-decoration: none;
    display: inline;
    margin-right: 1rem;
    font-style: normal;
    font-weight: normal;
    font-size: 13px;
    line-height: 19px;
    letter-spacing: 0.75px;
    color: #535353;
}

.view-more {
    font-style: normal;
    font-weight: normal;
    font-size: 20px;
    line-height: 32px;
    text-align: right;
    letter-spacing: 0.02em;
    color: #02be20;
    text-decoration: underline;
    cursor: pointer;
    /* margin: 1rem 8rem 3rem 5rem; */
}
.icons {
    margin-top: 0.5rem;
}
.icons ul li {
    background: rgba(8, 128, 75, 0.08);
    border-radius: 38px;
    padding: 0.3rem;
}
/* @media screen and (max-width: 768px) {
    .style-container {
        margin: 1rem;
    }
    .card {
        width: 100%;
    }
    .top-down {
        margin-top: 0.5rem;
    }
    .view-more {
        margin: 1rem 1rem 1rem 5rem;
    }
} */

/* cities */
.home-container {
    background: rgba(42, 0, 162, 0.03);
    padding: 1rem 0 4rem 0;
}
.style-container {
    margin: 3rem 5rem 0 8rem;
}
.header-home {
    font-style: normal;
    font-weight: bold;
    font-size: 26px;
    line-height: 37px;
    text-align: center;
    letter-spacing: 0.1em;
    color: #5e5c5c;
}
.border-line {
    margin: auto;
    width: 161px;
    height: 5px;
    background: #02be20;
}
.city {
    font-style: normal;
    font-weight: normal;
    font-size: 12px;
    line-height: 17px;
    text-align: center;
    letter-spacing: 0.02em;
    color: #000000;
}
.title {
    font-style: normal;
    font-weight: bold;
    font-size: 18px;
    line-height: 28px;
    letter-spacing: 0.02em;
    color: #000000;
    margin-top: 0.5rem;
}
.price {
    font-style: normal;
    font-weight: bold;
    font-size: 16px;
    line-height: 26px;
    text-align: right;
    letter-spacing: 0.02em;
    color: #000000;
}
.card-footer {
    background: #02be20 !important;
    color: #fff;
    text-align: center;
    font-weight: bold;
    font-size: 14px;
    line-height: 20px;
    letter-spacing: 1.8px;
    text-transform: uppercase;
    cursor: pointer;
}
ul {
    padding: 0;
    margin: 0;
}
ul li {
    list-style-type: none;
    text-decoration: none;
    display: inline;
    margin-right: 1rem;
    font-style: normal;
    font-weight: normal;
    font-size: 13px;
    line-height: 19px;
    letter-spacing: 0.75px;
    color: #535353;
}

.view-more {
    font-style: normal;
    font-weight: normal;
    font-size: 20px;
    line-height: 32px;
    text-align: center;
    letter-spacing: 0.02em;
    color: #02be20;
    text-decoration: underline;
    cursor: pointer;
}
.icons {
    margin-top: 0.5rem;
}
.icons ul li {
    background: rgba(8, 128, 75, 0.08);
    border-radius: 38px;
    padding: 0.3rem;
}

/* propertymanagement */
.style-container {
    margin: 7rem 5rem 7rem 8rem;
}
@media screen and (max-width: 578px) {
    input {
    /* background: #eff0f7; */
    width: 70%;
    margin-right: 1rem;
}
    .grid {
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-gap: 1rem;
    }
    .carousel-item {
        height: auto;
    }
    .wrapper {
        background: white;
        height: 120.6vh;
        background-size: cover;
        background-position: center;
        margin-bottom: 22rem;
    }
    .btn-success {
        width: 100%;
        display: block;
        margin: auto;
        margin-top: 2.5rem;
        padding-top: 1rem;
        padding-bottom: 1rem;
        margin-bottom: 2.5rem;
        background-color: #08804b;
        font-size: 1rem;
    }
    .wrapper-content {
        margin: auto;
        width: 100%;
        padding-top: 2rem;
    }
    .wrapper-content-one {
        font-size: 40px;
        font-weight: bold;
        text-align: center;
    }
    .wrapper-content img {
        width: 1.5rem;
        margin-right: 0.8rem;
    }
    .wrapper-content-two {
        text-align: center;
        padding-top: 1.5rem;
    }
    .header-title {
        font-style: normal;
        font-weight: bold;
        font-size: 30px;
        line-height: 30px;
        text-align: center;
        letter-spacing: 0.02em;
        color: #08804b;
        /* text-shadow: 4px 4px 7px rgba(0, 0, 0, 0.25); */
        /* backdrop-filter: blur(44px); */
        text-transform: uppercase;
    }
    .header-text {
        font-style: normal;
        font-weight: normal;
        font-size: 16px;
        line-height: 35px;
        text-align: center;
        letter-spacing: 0.02em;
        color: #c9c9c9;
        margin-top: 0.2rem;
    }
    .search-session {
        padding: 1rem;
        display: block;
    }
    .stroke {
        display: none;
    }
    .btn-search {
        width: 100%;
    }
    .top-down {
        margin-top: 0.5rem;
    }
    .line-on-mobile {
        display: block;
        color: #afafaf;
    }

    /* propertymanagement */
    .style-container {
        margin: 1rem;
    }
}
@media screen and (min-width: 710px) and (max-width: 1024px) {
    .wrapper-content {
        margin: auto;
        width: 100%;
        padding-top: 1rem;
    }
    .btn-success {
        width: 100%;
        display: block;
        margin: auto;
        margin-top: 2.5rem;
        padding-top: 1rem;
        padding-bottom: 1rem;
        margin-bottom: 2.5rem;
        background-color: #08804b;
        font-size: 1rem;
    }
    .wrapper {
        background: white;
        height: 70vh;
        background-size: cover;
        background-position: center;
        margin-bottom: 9rem;
    }
    .wrapper-content img {
        width: 1.5rem;
        margin-right: 0.8rem;
    }
}

@media screen and (max-width: 1024px) {
    /* homesection */
    .style-container {
        margin: 1rem;
    }
    .card {
        width: 100%;
    }
    .view-more {
        margin: 1rem 1rem 1rem 5rem;
    }
    .top-down {
        margin-top: 0.5rem;
    }

    /* rentsection */
    .style-container {
        margin: 1rem;
    }
    .card {
        width: 100%;
    }
    .view-more {
        margin: 1rem 1rem 1rem 5rem;
    }
    .top-down {
        margin-top: 0.5rem;
    }

    /* cities */
    .style-container {
        margin: 1rem;
    }
    .card {
        width: 100%;
    }
    .top-down {
        margin-top: 0.5rem;
    }
    .wrapper {
        background: white;
        height: 40vh;
        background-size: cover;
        background-position: center;
    }
}
</style>