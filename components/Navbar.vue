<template>
    <div class="fixed-top" style="background: #fff" ref="navbar">
        <div class="container">
            <nav class="navbar navbar-expand-lg navbar-light">
                <nuxt-link to="/" class="navbar-brand"
                    ><img
                        src="/img/logo/logo.png"
                        alt=""
                        srcset=""
                        width="92px"
                        height="40px"
                /></nuxt-link>
                <button
                    class="navbar-toggler"
                    type="button"
                    data-toggle="collapse"
                    data-target="#navbarSupportedContent"
                    aria-controls="navbarSupportedContent"
                    aria-expanded="false"
                    aria-label="Toggle navigation"
                >
                    <span class="navbar-toggler-icon"></span>
                </button>

                <div
                    class="collapse navbar-collapse"
                    id="navbarSupportedContent"
                >
                    <ul class="navbar-nav ml-auto">
                        <li class="nav-item">
                            <a class="nav-link" href="#">Featured Listings</a>
                        </li>
                        <li class="nav-item">
                            <nuxt-link to="/about-us" class="nav-link"
                                >About Us</nuxt-link
                            >
                        </li>
                        <li class="nav-item">
                            <nuxt-link
                                :to="{ path: '/', hash: '#footer' }"
                                class="nav-link"
                                >Contact Us</nuxt-link
                            >
                        </li>
                    </ul>
                    <form class="form-inline my-2 my-lg-0">
                        <nuxt-link to="/login">
                            <div class="btn btn-login" type="submit">Login</div>
                        </nuxt-link>
                        <nuxt-link to="/signup">
                            <div class="btn btn-create ml-3" type="submit">
                                Create Account
                            </div>
                        </nuxt-link>
                    </form>
                </div>
            </nav>
        </div>
    </div>
</template>
<script>
export default {
    mounted() {
        // window.scroll = this.newScroll();
        var navbar = this.$refs.navbar;
        $(window).scroll(function () {
            if ($(window).scrollTop() >= 10) {
                navbar.classList.add("scroll");
            } else {
                navbar.classList.remove("scroll");
            }
        });
    },
};
</script>
<style  scoped>
@font-face {
    font-family: sofiaPro;
    src: url("/font/sofiaProRegular.ttf");
}
* {
    font-family: sofiaPro;
}
.style-container {
    margin: 0 5rem 0 8rem;
}
.btn-login {
    font-style: normal;
    font-weight: bold;
    font-size: 18px;
    line-height: 26px;
    letter-spacing: 1px;
    color: #08804b;
}
.btn-create {
    background: #08804b;
    border-radius: 8px;
    font-style: normal;
    font-weight: bold;
    font-size: 18px;
    line-height: 26px;
    letter-spacing: 1px;
    color: #ffffff;
}
.nav-link {
    font-style: normal !important;
    font-weight: normal !important;
    font-size: 16px !important;
    line-height: 32px;
    /* identical to box height */

    letter-spacing: 1px !important;

    color: rgba(10, 0, 39, 0.38) !important;
    margin-left: 2rem;
}
.navbar-nav {
    margin-right: 1rem !important;
}
.scroll {
    background: #fff;
    transition: 1s ease-in;
    box-shadow: 0px 10px -14px 14px #fff !important;
}
@media screen and (max-width: 768px) {
    .style-container {
        margin: 0;
    }
    .nav-link {
        margin-left: 0.5rem;
    }
}
@media screen and (min-width: 1000px) and (max-width: 1024px) {
    .style-container {
        margin: 1rem;
    }
}
</style>