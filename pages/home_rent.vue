<template>
    <div>
        <div class="wrapper">
            <div class="container">
                <div class="wrapper-content">
                    <div class="header-title">home at last</div>
                    <div class="header-text">
                        Your Home Realtors you can trust
                    </div>
                    <div class="button-edit">
                        <div class="">
                            <div>
                                <div class="btn btn-buy">BUY</div>
                                <div class="btn btn-rent">RENT</div>
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
            <div class="header-home">LOOKING FOR A PLACE CALLED HOME ?</div>
            <div class="border-line"></div>
            <!-- cards -->
            <div class="container">
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
                </div>
            </div>
             <div class="row mt-5">
                <div class="col-sm-12 col-md-12 col-lg-4">
                    <div class="card top-down shadow rounded">
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
                </div>
            </div>
            <!-- button More -->
            <div class="view-more mt-4">
                View More 
            </div>
            </div>
            
        </div>
    </div>
        <div class="container mb-3">
            <div class="header-home mt-3">FOR RENT</div>
            <div class="border-line"></div>
            <!-- cards -->
            <div class="mt-5">
                <div class="row">
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
                                    <div class="title">Three Bedroom Flat</div>
                                    <div>
                                        <span class="price">&#8358;4.5m</span
                                        >/plot
                                    </div>
                                </div>
                                <div class="icons">
                                    <ul>
                                        <li>
                                            <img
                                                src="/img/icon/icon_1.png"
                                                alt=""
                                                srcset=""
                                            />
                                        </li>
                                        <li>
                                            <img
                                                src="/img/icon/icon_2.png"
                                                alt=""
                                                srcset=""
                                            />
                                        </li>
                                        <li>
                                            <img
                                                src="/img/icon/icon_3.png"
                                                alt=""
                                                srcset=""
                                            />
                                        </li>
                                        <li>
                                            <img
                                                src="/img/icon/icon_4.png"
                                                alt=""
                                                srcset=""
                                            />
                                        </li>
                                    </ul>
                                </div>
                            </div>
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
                                        <span class="price">&#8358;4.5m</span
                                        >/plot
                                    </div>
                                </div>
                                <div class="icons">
                                    <ul>
                                        <li>
                                            <img
                                                src="/img/icon/icon_1.png"
                                                alt=""
                                                srcset=""
                                            />
                                        </li>
                                        <li>
                                            <img
                                                src="/img/icon/icon_2.png"
                                                alt=""
                                                srcset=""
                                            />
                                        </li>
                                        <li>
                                            <img
                                                src="/img/icon/icon_3.png"
                                                alt=""
                                                srcset=""
                                            />
                                        </li>
                                        <li>
                                            <img
                                                src="/img/icon/icon_4.png"
                                                alt=""
                                                srcset=""
                                            />
                                        </li>
                                    </ul>
                                </div>
                            </div>
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
                                        <span class="price">&#8358;4.5m</span
                                        >/plot
                                    </div>
                                </div>
                                <div class="icons">
                                    <ul>
                                        <li>
                                            <img
                                                src="/img/icon/icon_1.png"
                                                alt=""
                                                srcset=""
                                            />
                                        </li>
                                        <li>
                                            <img
                                                src="/img/icon/icon_2.png"
                                                alt=""
                                                srcset=""
                                            />
                                        </li>
                                        <li>
                                            <img
                                                src="/img/icon/icon_3.png"
                                                alt=""
                                                srcset=""
                                            />
                                        </li>
                                        <li>
                                            <img
                                                src="/img/icon/icon_4.png"
                                                alt=""
                                                srcset=""
                                            />
                                        </li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="row mt-5">
                    <div class="col-sm-12 col-md-12 col-lg-4">
                        <div class="card top-down shadow rounded">
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
                                        <span class="price">&#8358;4.5m</span
                                        >/plot
                                    </div>
                                </div>
                                <div class="icons">
                                    <ul>
                                        <li>
                                            <img
                                                src="/img/icon/icon_1.png"
                                                alt=""
                                                srcset=""
                                            />
                                        </li>
                                        <li>
                                            <img
                                                src="/img/icon/icon_2.png"
                                                alt=""
                                                srcset=""
                                            />
                                        </li>
                                        <li>
                                            <img
                                                src="/img/icon/icon_3.png"
                                                alt=""
                                                srcset=""
                                            />
                                        </li>
                                        <li>
                                            <img
                                                src="/img/icon/icon_4.png"
                                                alt=""
                                                srcset=""
                                            />
                                        </li>
                                    </ul>
                                </div>
                            </div>
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
                                        <span class="price">&#8358;4.5m</span
                                        >/plot
                                    </div>
                                </div>
                                <div class="icons">
                                    <ul>
                                        <li>
                                            <img
                                                src="/img/icon/icon_1.png"
                                                alt=""
                                                srcset=""
                                            />
                                        </li>
                                        <li>
                                            <img
                                                src="/img/icon/icon_2.png"
                                                alt=""
                                                srcset=""
                                            />
                                        </li>
                                        <li>
                                            <img
                                                src="/img/icon/icon_3.png"
                                                alt=""
                                                srcset=""
                                            />
                                        </li>
                                        <li>
                                            <img
                                                src="/img/icon/icon_4.png"
                                                alt=""
                                                srcset=""
                                            />
                                        </li>
                                    </ul>
                                </div>
                            </div>
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
                                        <span class="price">&#8358;4.5m</span
                                        >/plot
                                    </div>
                                </div>
                                <div class="icons">
                                    <ul>
                                        <li>
                                            <img
                                                src="/img/icon/icon_1.png"
                                                alt=""
                                                srcset=""
                                            />
                                        </li>
                                        <li>
                                            <img
                                                src="/img/icon/icon_2.png"
                                                alt=""
                                                srcset=""
                                            />
                                        </li>
                                        <li>
                                            <img
                                                src="/img/icon/icon_3.png"
                                                alt=""
                                                srcset=""
                                            />
                                        </li>
                                        <li>
                                            <img
                                                src="/img/icon/icon_4.png"
                                                alt=""
                                                srcset=""
                                            />
                                        </li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="view-more mt-4">View More</div>
        </div>
        <div class="home-container">
            <div class="header-home">POPULAR CITIES</div>
            <div class="border-line"></div>
            <!-- cards -->
            <div class="container mt-5">
                <div class="row">
                    <div class="col-sm-12 col-md-12 col-lg-4">
                        <div class="card shadow rounded">
                            <img
                                src="/img/home/home.png"
                                class="card-img-top"
                                alt="..."
                            />
                            <div class="card-body">
                                <font-awesome-icon
                                    :icon="['fa', 'map-marker']"
                                />
                                <span class="city">Uyo, Akwa Ibom</span>
                            </div>
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
                                <font-awesome-icon
                                    :icon="['fa', 'map-marker']"
                                />
                                <span class="city">Uyo, Akwa Ibom</span>
                            </div>
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
                                <font-awesome-icon
                                    :icon="['fa', 'map-marker']"
                                />
                                <span class="city">Uyo, Akwa Ibom</span>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="row mt-5">
                    <div class="col-sm-12 col-md-12 col-lg-4">
                        <div class="card top-down shadow rounded">
                            <img
                                src="/img/home/home.png"
                                class="card-img-top"
                                alt="..."
                            />
                            <div class="card-body">
                                <font-awesome-icon
                                    :icon="['fa', 'map-marker']"
                                />
                                <span class="city">Uyo, Akwa Ibom</span>
                            </div>
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
                                <font-awesome-icon
                                    :icon="['fa', 'map-marker']"
                                />
                                <span class="city">Uyo, Akwa Ibom</span>
                            </div>
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
                                <font-awesome-icon
                                    :icon="['fa', 'map-marker']"
                                />
                                <span class="city">Uyo, Akwa Ibom</span>
                            </div>
                        </div>
                    </div>
                </div>
                <!-- button More -->
                <!-- <div class="view-more mt-4">View More</div> -->
            </div>
        </div>
        <border-line />
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
export default {};
</script>

<style scoped>
    @font-face {
    font-family: sofiaPro;
    src: url("/font/sofiaProRegular.ttf");
}
* {
    font-family: sofiaPro;
}
.wrapper {
    background: linear-gradient(
            to right,
            rgba(0, 4, 23, 0.58),
            rgba(0, 4, 23, 0.58)
        ),
        url("/img/hero/hero.png");
    height: 91.6vh;
    background-size: cover;
    background-position: center;
}
.wrapper-content {
    margin: auto;
    width: 70%;
    padding-top: 20rem;
}
.header-title {
    font-style: normal;
    font-weight: bold;
    font-size: 64px;
    line-height: 58px;
    text-align: center;
    letter-spacing: 0.02em;
    color: #ffffff;
    /* text-shadow: 4px 4px 7px rgba(0, 0, 0, 0.25); */
    /* backdrop-filter: blur(44px); */
    text-transform: uppercase;
}
.header-text {
    font-style: normal;
    font-weight: normal;
    font-size: 24px;
    line-height: 35px;
    text-align: center;
    letter-spacing: 0.02em;
    color: #c9c9c9;
    margin-top: 0.2rem;
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
}
.btn-rent {
    background: #ffffff;
    border-radius: 0px 4px 4px 0px;
    color: #08804b;
    padding-left: 3rem;
    padding-right: 3rem;
    position: relative;
    left: -4px;
}
.search-session {
    background: #fff;
    padding: 1rem;
    display: flex;
    justify-content: space-between;
    margin-top: 2rem;
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
    .wrapper {
        background: linear-gradient(
                to right,
                rgba(0, 4, 23, 0.58),
                rgba(0, 4, 23, 0.58)
            ),
            url("/img/hero/hero.png");
        height: 91.6vh;
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
        font-size: 48px;
        line-height: 58px;
        text-align: center;
        letter-spacing: 0.02em;
        color: #ffffff;
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
        padding-top: 16rem;
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
}
</style>