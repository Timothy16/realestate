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
                <h5 class="footer-text">QUICK LINKS</h5>
                <ul>
                    <li>Featured Listings</li>
                    <li>About Us</li>
                    <li>Contact Us</li>
                </ul>
                <h5 class="footer-text">FOLLOW US</h5>
                <ul>
                    <li><img src="/img/icon/ins.png" alt="" srcset="" class="footer-img"></li>
                    <li><img src="/img/icon/lin.png" alt="" srcset="" class="footer-img"></li>
                    <li><img src="/img/icon/fa.png" alt="" srcset="" class="footer-img"></li>
                    <li><img src="/img/icon/tw.png" alt="" srcset="" class="footer-img"></li>
                </ul>
                <hr>
                <p class="text-1">Copyright 2021 - JayCee & Jay Ltd. All Rights Reserved.</p>
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
    font-size: 17px;
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
    font-weight: bold;
    font-size: 15px;
    line-height: 22px;
    letter-spacing: 1.5px;
    color: #e9fff5;
    margin: 0 1.5rem 0 0;
}
.footer-text{
    color:#08804B;
    font-weight: bold;
}
.footer-img{
    width: 2rem;
    margin-top: 0.7rem;
}
hr{
    border: 1px solid rgba(233, 255, 245, 0.35);
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
    width: 90%;
    margin-top: 1rem;
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
    .footer-img{
    width: 2rem;
    margin-top: 0.7rem;
}
}
</style>