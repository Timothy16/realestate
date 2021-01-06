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
                <ul>
                    <li>Featured Listings</li>
                    <li>About Us</li>
                    <li>Contact Us</li>
                </ul>
            </div>
        </div>
    </div>
</template>
<style scoped>
.line {
    height: 10px;
    background: #02be20;
}
.footer-bg {
    background: #001e11;
    padding: 5rem 0 2rem 0;
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
    font-weight: bold;
    font-size: 16px;
    line-height: 22px;
    letter-spacing: 1.5px;
    color: #e9fff5;
    margin: 0 1.5rem 0 0;
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