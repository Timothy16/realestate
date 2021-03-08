<template>
    <div>
        <div class="container">
            <div
                id="carouselExampleIndicators"
                class="carousel slide"
                data-ride="carousel"
                data-interval="1000"
            >
                <ol class="carousel-indicators">
                    <li :class="{imageDisplay : this.displayInfo.photo_main === null}"
                        data-target="#carouselExampleIndicators"
                        data-slide-to="0"
                        class="active"
                    ></li>
                    <li :class="{imageDisplay : this.displayInfo.photo_1 === null}"
                        data-target="#carouselExampleIndicators"
                        data-slide-to="1"
                    ></li>
                    <li :class="{imageDisplay : this.displayInfo.photo_2 === null}"
                        data-target="#carouselExampleIndicators"
                        data-slide-to="2"
                    ></li>
                    <li :class="{imageDisplay : this.displayInfo.photo_3 === null}"
                        data-target="#carouselExampleIndicators"
                        data-slide-to="3"
                    ></li>
                    <li :class="{imageDisplay : this.displayInfo.photo_4 === null}"
                        data-target="#carouselExampleIndicators"
                        data-slide-to="4"
                    ></li>
                    <li :class="{imageDisplay : this.displayInfo.photo_5 === null}"
                        data-target="#carouselExampleIndicators"
                        data-slide-to="5"
                    ></li>
                    <li :class="{imageDisplay : this.displayInfo.photo_6 === null}"
                        data-target="#carouselExampleIndicators"
                        data-slide-to="6"
                    ></li>
                    
                </ol>
                <div class="carousel-inner">
                    <div class="carousel-item active" :class="{imageDisplay : this.displayInfo.photo_main === null}">
                        <img
                            class="d-block w-100"
                            :src="this.displayInfo.photo_main"
                            alt="First slide"
                        />
                    </div>
                    <div class="carousel-item" :class="{imageDisplay : this.displayInfo.photo_1 === null}">
                        <img
                            class="d-block w-100"
                            :src="this.displayInfo.photo_1"
                            alt="no image"
                        />
                    </div>
                     <div class="carousel-item" :class="{imageDisplay : this.displayInfo.photo_2 === null}">
                        <img
                            class="d-block w-100"
                            :src="this.displayInfo.photo_2"
                            alt="no image"
                        />
                    </div>
                     <div class="carousel-item" :class="{imageDisplay : this.displayInfo.photo_3 === null}">
                        <img
                            class="d-block w-100"
                            :src="this.displayInfo.photo_3"
                            alt="no image"
                        />
                    </div>
                     <div class="carousel-item" :class="{imageDisplay : this.displayInfo.photo_4 === null}">
                        <img
                            class="d-block w-100"
                            :src="this.displayInfo.photo_4"
                            alt="no image"
                        />
                    </div>
                     <div class="carousel-item" :class="{imageDisplay : this.displayInfo.photo_5 === null}">
                        <img
                            class="d-block w-100"
                            :src="this.displayInfo.photo_5"
                            alt="no image"
                        />
                    </div>
                     <div class="carousel-item" :class="{imageDisplay : this.displayInfo.photo_6 === null}">
                        <img
                            class="d-block w-100"
                            :src="this.displayInfo.photo_6"
                            alt="no image"
                        />
                    </div>
                    <!-- <div class="carousel-item">
                        <img
                            class="d-block w-100"
                            :src="this.displayInfo.photo_2"
                            alt="Third slide"
                        />
                    </div> -->
                </div>
                <a
                    class="carousel-control-prev"
                    href="#carouselExampleIndicators"
                    role="button"
                    data-slide="prev"
                >
                    <span
                        class="carousel-control-prev-icon"
                        aria-hidden="true"
                    ></span>
                    <span class="sr-only">Previous</span>
                </a>
                <a
                    class="carousel-control-next"
                    href="#carouselExampleIndicators"
                    role="button"
                    data-slide="next"
                >
                    <span
                        class="carousel-control-next-icon"
                        aria-hidden="true"
                    ></span>
                    <span class="sr-only">Next</span>
                </a>
            </div>
        
        <div class="wrapper">
            <div class="container">
                <div class="wrapper-content">
                    <div class="row">
                        <div
                            class="col-sm-12 col-md-6 col-lg-6 wrapper-content-one"
                        >
                            <h6>{{this.displayInfo.address}}, {{this.displayInfo.city}}, {{this.displayInfo.state}}</h6>
                            <h2>{{this.displayInfo.title}}</h2>
                        </div>
                        <div
                            class="col-sm-12 col-md-6 col-lg-6 wrapper-content-two"
                        >
                            <span class="wrapper-content-two-one">&#8358;{{this.displayInfo.price}}</span
                            ><span class="wrapper-content-two-two"></span>
                        </div>
                    </div>
                    <div class="grid mt-5">
                        <div class="">
                            <img
                                src="/img/icon/icon_12.png"
                                alt=""
                                srcset=""
                            /><span>{{this.displayInfo.bedrooms}} Bedrooms</span>
                        </div>
                        <div class="">
                            <img
                                src="/img/icon/icon_13.png"
                                alt=""
                                srcset=""
                            /><span>{{this.displayInfo.bathrooms}} Restrooms</span>
                        </div>
                        <div class="">
                            <img
                                src="/img/icon/icon_5.png"
                                alt=""
                                srcset=""
                            /><span>Electricity</span>
                        </div>
                        <div class="">
                            <img
                                src="/img/icon/icon_6.png"
                                alt=""
                                srcset=""
                            /><span>Home Library</span>
                        </div>
                    </div>
                    <div class="grid mt-4">
                        <div class="">
                            <img
                                src="/img/icon/icon_7.png"
                                alt=""
                                srcset=""
                            /><span>{{this.displayInfo.garage}} Parking Lots</span>
                        </div>
                        <div class="">
                            <img
                                src="/img/icon/icon_8.png"
                                alt=""
                                srcset=""
                            /><span>Eatery</span>
                        </div>
                        <div class="">
                            <img
                                src="/img/icon/icon_10.png"
                                alt=""
                                srcset=""
                            /><span>{{this.displayInfo.sqft}} Square Fts</span>
                        </div>
                        <div class="">
                            <img
                                src="/img/icon/icon_11.png"
                                alt=""
                                srcset=""
                            /><span>Quiet Environment</span>
                        </div>
                    </div>
                    <!-- Button trigger modal -->
                    <button
                        type="button"
                        class="btn btn-success"
                        data-bs-toggle="modal"
                        data-bs-target="#exampleModal"
                    >
                        Make Enquiry
                    </button>

                    <!-- Modal -->
                    <div
                        class="modal fade"
                        id="exampleModal"
                        tabindex="-1"
                        aria-labelledby="exampleModalLabel"
                        aria-hidden="true"
                    >
                        <div class="modal-dialog">
                            <div class="modal-content">
                                <div class="modal-header">
                                    <p
                                        class="modal-title"
                                        id="exampleModalLabel"
                                    >
                                        Make an Enquiry
                                    </p>
                                    <button
                                        type="button"
                                        class="close"
                                        data-bs-dismiss="modal"
                                        aria-label="Close"
                                    >
                                        <span aria-hidden="true">&times;</span>
                                    </button>
                                </div>
                                <div class="modal-body">
                                    <form action="" @submit.prevent="messages">
                                        <div class="mt-1">
                                            <label for="">Property Name</label>
                                            <input
                                                type="text"
                                                class="form-control"
                                                placeholder="Ewet Housing Estate"
                                                required
                                                v-model="messageInfo.rent"
                                            />
                                        </div>
                                        <div>
                                            <label for="">Name</label>
                                            <input
                                                type="text"
                                                class="form-control"
                                                placeholder="John Doe"
                                                 required
                                                v-model="messageInfo.name"
                                            />
                                        </div>
                                        
                                        <div class="mt-1">
                                            <label for="">Email Address</label>
                                            <input
                                                type="email"
                                                class="form-control"
                                                placeholder="johndoe@gmail.com"
                                                required
                                                v-model="messageInfo.email"
                                            />
                                        </div>
                                        <div class="mt-1">
                                            <label for="">Phone Number</label>
                                            <input
                                                type="text"
                                                class="form-control"
                                                placeholder="08012345678"
                                                required
                                                v-model="messageInfo.phone"
                                            />
                                        </div>
                                        <div class="mt-1">
                                            <label for="">Message</label>
                                            <textarea
                                                name=""
                                                id=""
                                                class="form-control w-100"
                                                required
                                                v-model="messageInfo.message"
                                            ></textarea>
                                        </div>
                                        <div class="modal-footer">
                                    <button
                                        type="submit"
                                        class="btn btn-send mt-4 w-100"
                                    >
                                        Message Us
                                    </button>
                                </div>
                                    </form>
                                </div>
                                <div class="modal-footer">
                                    
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div>
            <div class="container">
                <PropertyManagment />
            </div>
        </div>
        </div>
    </div>
</template>

<script>
import ElementUI from 'element-ui';
import 'element-ui/lib/theme-chalk/index.css';
export default {
    data(){
        return{
            displayInfo:{},
            messageInfo : {
                name:'',
                email : '',
                phone : '',
                message : '',
                rent_id: '1',
                rent: '',
                user_id: '1',
            },
        }
    },
    mounted(){
        this.getDisplayInfo()
    },
    methods:{
        getDisplayInfo(){
            this.$axios.get(`https://jayceeandjay.online/Rents/${this.$route.params.id}`).then((res)=> {
               this.displayInfo=res.data;
               console.log(this.displayInfo);
               this.messageInfo.rent = this.displayInfo.title;
         }) 
        },
         messages(){
             this.$axios.post('https://jayceeandjay.online/rentcontact/', this.messageInfo,
              {headers : {'Content-Type':'application/json'}}).then((res)=> {
                  this.$message({
            message:"Message Sent!",
            type: "success",
          });this.messageInfo={};
                this.messageResponse=res.data;
               console.log(this.messageResponse);
               

            }).catch((error) => {
          console.log(error);
          
        });
           
        },
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
.imageDisplay{
    display : none
}
.carousel-item img{
    height: 500px !important;
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
label {
    color: #002817;
    font-style: normal;
    font-weight: bold;
}
input {
    background: #eff0f7;
    width: 70%;
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
    /* height: 65vh; */
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
    text-align: center;
    letter-spacing: 0.06em;
    color: #afafaf;
    margin-right: 0.5rem;
}
input {
    outline: none;
    border: none;
    width: 100%;
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
    padding: 3rem 0 3rem 0;
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
    padding: 3rem 0 4rem 0;
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
    .wrapper-content-one h2 {
    font-size: 20px;
    font-weight: bold;
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
        /* height: 120.6vh; */
        background-size: cover;
        background-position: center;
        /* margin-bottom: 22rem; */
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
        /* height: 70vh; */
        background-size: cover;
        background-position: center;
        /* margin-bottom: 9rem; */
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
        /* height: 40vh; */
        background-size: cover;
        background-position: center;
    }
}
</style>