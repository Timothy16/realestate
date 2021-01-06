<template>
    <div>
        <div
            id="carouselExampleIndicators"
            class="carousel slide"
            data-ride="carousel"
        >
            <ol class="carousel-indicators">
                <li
                    data-target="#carouselExampleIndicators"
                    data-slide-to="0"
                    class="active"
                ></li>
                <li
                    data-target="#carouselExampleIndicators"
                    data-slide-to="1"
                ></li>
                <li
                    data-target="#carouselExampleIndicators"
                    data-slide-to="2"
                ></li>
            </ol>
            <div class="carousel-inner">
                <div class="carousel-item active">
                    <img
                        class="d-block w-100"
                        src="/img/home/home.png"
                        alt="First slide"
                    />
                    <div class="carousel-caption d-none d-md-block">
                        <h5>Le Meridien Estate</h5>
                    </div>
                </div>
                <div class="carousel-item">
                    <img
                        class="d-block w-100"
                        src="/img/home/home.png"
                        alt="Second slide"
                    />
                    <div class="carousel-caption d-none d-md-block">
                        <h5>Le Meridien Estate</h5>
                    </div>
                </div>
                <div class="carousel-item">
                    <img
                        class="d-block w-100"
                        src="/img/home/home.png"
                        alt="Third slide"
                    />
                    <div class="carousel-caption d-none d-md-block">
                        <h5>Le Meridien Estate</h5>
                    </div>
                </div>
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
    </div>
</template>

<style scoped>
@font-face {
    font-family: sofiaPro;
    src: url("/font/sofiaProRegular.ttf");
}
* {
    font-family: sofiaPro;
}
.carousel-item {
    height: 400px;
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
@media screen and (max-width: 578px) {
    .carousel-item {
        height: auto;
    }
}
</style>