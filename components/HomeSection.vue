<template>
    <div class="home-container">
        <div class="" >
            <div class="header-home">LOOKING FOR A PLACE CALLED HOME ?</div>
            <div class="border-line"></div>
            <!-- cards -->
            <div class="container">
            <div class="row mt-5" v-if="salesItems.length > 0">
                <div class="col-sm-12 col-md-12 col-lg-4 mb-2" v-for="(info,index) in salesItems" :key="index">
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
                <!-- <div class="col-sm-12 col-md-12 col-lg-4">
                    <div class="card top-down rounded shadow">
                        <img
                            src="/img/home/home.png"
                            class="card-img-top"
                            alt="..."
                        />
                        <div class="card-body">
                            <span class="city">Uyo, Akwa Ibom</span>
                            <div class="d-flex justify-content-between">
                                <div class="title">Three Bedroom Flat</div>
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
                            <p class="mt-1">
                               <ul>
                                   <li>
                                       Three Bedroom
                                   </li>
                                   <li>
                                       Three Restroom
                                   </li>
                               </ul>
                            </p>
                             <p class="mt-1">
                               <ul>
                                   <li>
                                      24 Square Fts
                                   </li>
                                   <li style="margin-left : .7rem">
                                      CCTV Surveillance
                                   </li>
                               </ul>
                            </p>
                        </div>
                        <div class="card-footer">More Information</div>
                    </div>
                </div>
                <div class="col-sm-12 col-md-12 col-lg-4">
                    <div class="card top-down rounded shadow">
                        <img
                            src="/img/home/home.png"
                            class="card-img-top"
                            alt="..."
                        />
                        <div class="card-body">
                            <span class="city">Uyo, Akwa Ibom</span>
                            <div class="d-flex justify-content-between">
                                <div class="title">Three Bedroom Flat</div>
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
                            <p class="mt-1">
                               <ul>
                                   <li>
                                       Three Bedroom
                                   </li>
                                   <li>
                                       Three Restroom
                                   </li>
                               </ul>
                            </p>
                             <p class="mt-1">
                               <ul>
                                   <li>
                                      24 Square Fts
                                   </li>
                                   <li style="margin-left : .7rem">
                                      CCTV Surveillance
                                   </li>
                               </ul>
                            </p>
                        </div>
                        <div class="card-footer">More Information</div>
                    </div>
                </div> -->
            </div>
            <div class="mt-5" v-else>
                <Loader />
            </div>
            <!-- button More -->
            <nuxt-link to="/more_sales"><div class="view-more mt-4">
                View More 
            </div></nuxt-link>
            
            </div>
            
        </div>
    </div>
</template>
<script>
export default {
    data() {
        return {
            salesItems: {},
        };
    },
    mounted() {
        this.getSalesItems();
    },
    methods: {
        getSalesItems() {
            this.$axios
                .get("https://jayceeandjay.online/sales", {
                    headers: { "Content-Type": "application/json" },
                })
                .then((res) => {
                    this.salesItems = res.data.results;
                    console.log(this.salesItems);
                });
        },
         displayInfo(info){
         this.$router.push(`/sales/${info}`)
    }
}
}
</script>
<style scoped>
@font-face {
    font-family: sofiaPro;
    src: url("/font/sofiaProRegular.ttf");
}
* {
    font-family: sofiaPro;
}
a {
    text-decoration: none !important;
}
.home-container {
    background: rgba(42, 0, 162, 0.03);
    padding: 3rem 0 3rem 0;
}
.box-down {
    margin-top: 3rem;
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
@media screen and (max-width: 1024px) {
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

    .box-down {
        margin-top: 1rem;
    }
}
</style>