<template>
    <div id="footer">
        <div class="line"></div>
        <div class="footer-bg">
            <div>
                <img src="/img/logo/logo.png" alt="" srcset="" />
            </div>
            <p class="text-1">
                <span class="break"
                    >7a Ero Close, Idado Estate, Lekki Phase 1.Opposite Igbo
                    Efon Bus stop, Lekki Expressway.</span
                >
                Eti Osa LGA, Lagos State.
            </p>
            <p class="text-1">07063499427, 08026674533</p>
            <div class="mt-3">
                <div class="quick-link mb-2">QUICK LINKS</div>
                <ul class="mt-2">
                    <li>Featured Listings</li>
                    <li>About Us</li>
                    <li>Contact Us</li>
                </ul>
            </div>
            <div class="mt-3">
                <div class="quick-link">FOLLOW US</div>
                <ul class="mt-2">
                    <li>
                        <img src="/img/icon/facebook.png" alt="" srcset="" />
                    </li>
                    <li>
                        <img src="/img/icon/linkdin.png" alt="" srcset="" />
                    </li>
                    <li>
                        <img src="/img/icon/instagram.png" alt="" srcset="" />
                    </li>
                    <li>
                        <img src="/img/icon/twitter.png" alt="" srcset="" />
                    </li>
                </ul>
            </div>
            <div class="container">
                <hr class="line-footer" />
            </div>
            <div class="copy-right">
                copyright 2021 - JayCee & Jay Ltd. All rights reserved
            </div>
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
.line {
    height: 10px;
    background: #02be20;
}
.footer-bg {
    background: #001e11;
    padding: 5rem 0 1rem 0;
    text-align: center;
}
.text-1 {
    font-style: normal;
    font-weight: normal;
    font-size: 18px;
    line-height: 24px;
    color: rgba(233, 255, 245, 0.76);
    margin-top: 0.8rem;
}
.break::after {
    content: "\a";
    white-space: pre;
}
ul li {
    list-style-type: none;
    text-decoration: none;
    display: inline;
    font-style: normal;
    /* font-weight: bold; */
    font-size: 16px;
    line-height: 22px;
    letter-spacing: 1.5px;
    color: #e9fff5;
    margin: 0 1.5rem 0 0;
}
.quick-link {
    font-style: normal;
    font-weight: bold;
    font-size: 18px;
    line-height: 24px;
    text-align: center;
    letter-spacing: 0.06em;
    color: #08804b;
}
.line-footer {
    border: 1px solid rgba(233, 255, 245, 0.35);
}
.copy-right {
    font-style: normal;
    font-weight: normal;
    font-size: 18px;
    line-height: 24px;
    text-align: center;
    letter-spacing: 0.05em;
    color: rgba(233, 255, 245, 0.76);
}
@media screen and (max-width: 578px) {
    ul li {
        list-style-type: none;
        text-decoration: none;
        display: inline;
        font-style: normal;
        font-weight: bold;
        font-size: 16px;
        line-height: 22px;
        letter-spacing: 1.5px;
        color: #e9fff5;
        margin: 0 1.5rem 0 0;
    }
}
</style>