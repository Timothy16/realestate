<template>
    <div>
        <div class="wrapper">
            <div class="container">
                <div class="wrapper-content">
                    <div class="header-text">
                        FOUND 300 SEARCH RESULTS FOR
                    </div>
                    <div class="header-title">UYO, 4 ROOMS, AKWA IBOM, SELL</div>
                    <div class="button-edit">
                        <div class="">
                            <div>
                                <div class="btn btn-rent">BUY</div>
                                <div class="btn btn-buy">RENT</div>
                            </div>
                        </div>
                    </div>
                    <div class="search-session rounded">
                        <div class="d-flex">
                            <span style="margin-top: 0.6rem"
                                ><font-awesome-icon :icon="['fa', 'search']"
                            /></span>
                            <input
                                class="pl-3"
                                type="text"
                                placeholder="Search City, Street,Apartment"
                            />
                        </div>
                        <div class="stroke">|</div>
                        <hr class="line-on-mobile" />
                        <div class="top-down">
                            <select class="" id="options">
                                <option selected disabled>Rooms</option>
                                <option>2</option>
                                <option>3</option>
                                <option>4</option>
                            </select>
                        </div>
                        <div class="stroke">|</div>
                        <hr class="line-on-mobile" />
                        <div class="top-down">
                            <select class="" id="options">
                                <option selected disabled>State</option>
                                <option>2</option>
                            </select>
                        </div>
                        <div class="btn btn-search top-down">Search</div>
                    </div>
                    <div class="angle-edit">
                        <font-awesome-icon
                            :icon="['fa', 'angle-double-down']"
                        />
                    </div>
                </div>
            </div>
            
        </div>
        <div class="home-container">
        <div class="">
            <!-- cards -->
            <div class="container">
            <div class="row mt-2" v-for="(info,index) in salesItems" :key="index">
                <div class="col-sm-12 col-md-12 col-lg-4">
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
                        <nuxt-link to="/about_property">
                        <div class="card-footer">More Information</div>
                        </nuxt-link>
                    </div>
                    </div>
                <!-- <div class="col-sm-12 col-md-12 col-lg-4">
                    <div class="card shadow rounded">
                        <img
                            src="/img/home/home.png"
                            class="card-img-top"
                            alt="..."
                        />
                        <div class="card-body">
                            <span class="city">Uyo, Akwa Ibom</span>
                            <div class="d-flex justify-content-between">
                                <div class="title">Ibom Estate</div>
                                <div>
                                    <span class="price">&#8358;4.5m</span>/plot
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
                        </div>
                    </div>
                </div>
                <div class="col-sm-12 col-md-12 col-lg-4">
                    <div class="card shadow rounded">
                        <img
                            src="/img/home/home.png"
                            class="card-img-top"
                            alt="..."
                        />
                        <div class="card-body">
                            <span class="city">Uyo, Akwa Ibom</span>
                            <div class="d-flex justify-content-between">
                                <div class="title">Ibom Estate</div>
                                <div>
                                    <span class="price">&#8358;4.5m</span>/plot
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
                        </div>
                    </div>
                </div> -->
            </div>
             <!-- <div class="row mt-5">
                <div class="col-sm-12 col-md-12 col-lg-4">
                    <div class="card shadow rounded">
                        <img
                            src="/img/home/home.png"
                            class="card-img-top"
                            alt="..."
                        />
                        <div class="card-body">
                            <span class="city">Uyo, Akwa Ibom</span>
                            <div class="d-flex justify-content-between">
                                <div class="title">Ibom Estate</div>
                                <div>
                                    <span class="price">&#8358;4.5m</span>/plot
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
                        </div>
                    </div>
                </div>
                <div class="col-sm-12 col-md-12 col-lg-4">
                    <div class="card shadow rounded">
                        <img
                            src="/img/home/home.png"
                            class="card-img-top"
                            alt="..."
                        />
                        <div class="card-body">
                            <span class="city">Uyo, Akwa Ibom</span>
                            <div class="d-flex justify-content-between">
                                <div class="title">Ibom Estate</div>
                                <div>
                                    <span class="price">&#8358;4.5m</span>/plot
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
                        </div>
                    </div>
                </div>
                <div class="col-sm-12 col-md-12 col-lg-4">
                    <div class="card shadow rounded">
                        <img
                            src="/img/home/home.png"
                            class="card-img-top"
                            alt="..."
                        />
                        <div class="card-body">
                            <span class="city">Uyo, Akwa Ibom</span>
                            <div class="d-flex justify-content-between">
                                <div class="title">Ibom Estate</div>
                                <div>
                                    <span class="price">&#8358;4.5m</span>/plot
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
                        </div>
                    </div>
                </div>
            </div>
            <div class="row mt-5">
                <div class="col-sm-12 col-md-12 col-lg-4">
                    <div class="card shadow rounded">
                        <img
                            src="/img/home/home.png"
                            class="card-img-top"
                            alt="..."
                        />
                        <div class="card-body">
                            <span class="city">Uyo, Akwa Ibom</span>
                            <div class="d-flex justify-content-between">
                                <div class="title">Ibom Estate</div>
                                <div>
                                    <span class="price">&#8358;4.5m</span>/plot
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
                        </div>
                    </div>
                </div>
                <div class="col-sm-12 col-md-12 col-lg-4">
                    <div class="card shadow rounded">
                        <img
                            src="/img/home/home.png"
                            class="card-img-top"
                            alt="..."
                        />
                        <div class="card-body">
                            <span class="city">Uyo, Akwa Ibom</span>
                            <div class="d-flex justify-content-between">
                                <div class="title">Ibom Estate</div>
                                <div>
                                    <span class="price">&#8358;4.5m</span>/plot
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
                        </div>
                    </div>
                </div>
                <div class="col-sm-12 col-md-12 col-lg-4">
                    <div class="card shadow rounded">
                        <img
                            src="/img/home/home.png"
                            class="card-img-top"
                            alt="..."
                        />
                        <div class="card-body">
                            <span class="city">Uyo, Akwa Ibom</span>
                            <div class="d-flex justify-content-between">
                                <div class="title">Ibom Estate</div>
                                <div>
                                    <span class="price">&#8358;4.5m</span>/plot
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
                        </div>
                    </div>
                </div>
            </div> -->
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
                    <div class="form-edit">
        <div class="form-head">PROPERTY MANAGEMENT</div>
        <p class="mt-2">
            Great article. I wonder if there is a way this can be learned?
        </p>
        <form action="" @submit.prevent="message">
            <div>
                <input
                    type="text"
                    class="form-control input"
                    placeholder="Full Name"
                    v-model="messageInfo.name"
                />
            </div>
            <div class="mt-1">
                <input
                    type="email"
                    class="form-control input"
                    placeholder="Email Address"
                    v-model="messageInfo.email"
                />
            </div>
            <div class="mt-1">
                <input
                    type="text"
                    class="form-control input"
                    placeholder="Phone Number"
                    v-model="messageInfo.phone"
                />
            </div>
            <div class="mt-1">
                <textarea name="" 
                id="" 
                class="form-control input" 
                placeholder="Message"
                v-model="messageInfo.message"
                ></textarea>
            </div>
            <button class="btn btn-send mt-4" type="submit">Message Us</button>
        </form>
    </div>
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
            salesItems:{},
            messageResponse:{},
            messageInfo : {
                name:'',
                email : '',
                phone : '',
                message : '',
                sale_id: '1',
                sale: '2',
                user_id: '1',
            },
        }
    },
    mounted(){
        this.searchSalesItems()
    },
    methods:{
    searchSalesItems(){
        this.$axios.get("https://api.jayceeandjay.com/salesearch", {headers : {'Content-Type':'application/json'}}).then((res)=> {
               this.salesItems=res.data.results;
               console.log(this.salesItems)
         }) 
    },
    message(){
             this.$axios.post('https://api.jayceeandjay.com/salecontact/', this.messageInfo,
              {headers : {'Content-Type':'application/json'}}).then((res)=> {
                this.messageResponse=res.data;
               console.log(this.messageResponse)

            })
           
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
.input {
    background: #eff0f7;
    width: 70%;
    margin-bottom: 1rem;
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
.wrapper {
    background: white;
    height: 50vh;
    margin-bottom: 1rem;
    background-size: cover;
    background-position: center;
}
.wrapper-content {
    margin: auto;
    width: 70%;
    padding-top: 2rem;
}
.header-title {
    font-style: normal;
    font-weight: bold;
    font-size: 38px;
    line-height: 38px;
    text-align: center;
    letter-spacing: 0.02em;
    color: #08804B;
;
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
    background:#EBF5F1;
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
    border: #EBF5F1 1px solid;
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
    .input{
    width: 100%;
}
    .wrapper {
        background: white;
        height: 91.6vh;
        margin-bottom: 17rem;
        background-size: cover;
        background-position: center;
    }
    .wrapper-content {
        margin: auto;
        width: 100%;
        padding-top: 2rem;
    }
    .header-title {
        font-style: normal;
        font-weight: bold;
        font-size: 30px;
        line-height: 30px;
        text-align: center;
        letter-spacing: 0.02em;
        color:  #08804B;
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
    .form-edit {
        padding: 1rem;
    }
    input {
        width: 100%;
    }
    textarea {
        width: 100%;
    }
    .btn-send {
        width: 100%;
    }
    .form-head {
        font-style: normal;
        font-weight: bold;
        font-size: 18px;
        line-height: 28px;
        letter-spacing: 0.03em;
        text-transform: uppercase;
        color: #002817;
        margin-top: 1rem;
    }
}
@media screen and (min-width: 710px) and (max-width: 1024px) {
    .wrapper-content {
        margin: auto;
        width: 100%;
        padding-top: 1rem;
    }
    .form-edit{
        margin-top: 7vh;
    }
    .wrapper {
        background: white;
        height: 60vh;
        background-size: cover;
        background-position: center;
        margin-bottom: 3rem;
    }
     .form-edit {
        padding: 0;
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
        height: 50vh;
        background-size: cover;
        background-position: center;
    }
}
</style>