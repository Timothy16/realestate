<template>
    <div>
        <div class="style-container">
            <nav class="navbar navbar-expand-lg navbar-light">
                <a class="navbar-brand" href="#"
                    ><img
                        src="/img/logo/logo.png"
                        alt=""
                        srcset=""
                        width="92px"
                        height="40px"
                /></a>
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
                            <a class="nav-link" href="#">Contact Us</a>
                        </li>
                    </ul>
                    <form class="form-inline my-2 my-lg-0">
                        <div class="btn btn-login" type="submit">Login</div>
                        <div class="btn btn-create ml-3" type="submit">
                            Create Account
                        </div>
                    </form>
                </div>
            </nav>
        </div>
    </div>
</template>
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
    font-size: 22px !important;
    line-height: 32px;
    /* identical to box height */

    letter-spacing: 1px !important;

    color: rgba(10, 0, 39, 0.38) !important;
    margin-left: 2rem;
}
.navbar-nav {
    margin-right: 1rem !important;
}
</style>