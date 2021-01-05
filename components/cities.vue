<template>
    <div class="">
        <div class="home-container">
            <div class="header-home">POPULAR CITIES</div>
            <div class="border-line"></div>
            <!-- cards -->
            <div class="style-container mt-5">
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
                        <div class="card rounded shadow">
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
                        <div class="card rounded shadow">
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
                        <div class="card rounded shadow">
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
                        <div class="card rounded shadow">
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
    </div>
</template>

<style scoped>
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
.card {
    width: 394px;
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
</style>