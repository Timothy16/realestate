<template>
    <div>
        <div class="style-container">
            <div class="row">
                <div class="col-sm-12 col-md-12 col-lg-6">
                    <div class="about-header">About Us</div>
                    <div class="line-about"></div>
                    <div class="mt-3">
                        <p class="text-edit">
                            At JAYCEE & JAY LTD, we know what works. We've
                            developed a proven, hands-on approach to management
                            that's served the community for over 7 years.
                        </p>
                        <p class="text-edit">
                            JAYCEE & JAY agents are current in all areas of
                            Management and we are 100% committed to serving our
                            clients. Contact us today and make JAYCEE & JAY LTD
                            your property management company of choice.
                        </p>
                        <p class="text-edit">
                            Trusted by homeowners, investment owners, real
                            estate professionals and developers, we are
                            committed to excellence and with highest quality of
                            customer support.
                        </p>
                    </div>
                </div>
                <div class="col-sm-12 col-md-12 col-lg-6">
                    <img
                        src="/img/home/team.png"
                        class="img-fluid"
                        alt=""
                        srcset=""
                    />
                </div>
            </div>
        </div>
        <div class="vision">
            <div class="vision-text">Our Vision</div>
            <div class="line-2"></div>
            <p class="text-edit text-center mt-1">
                <span class="break">
                    The vision of JAYCEE & JAY LTD is to achieve the highest
                    possible standards of the real estate market while</span
                >
                establishing our agency as the premier and preferred real estate
                company in Nigeria.
            </p>
        </div>
        <property-managment />
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
.style-container {
    margin: 10rem 5rem 3rem 8rem;
}
.about-header {
    font-style: normal;
    font-weight: bold;
    font-size: 28px;
    line-height: 28px;
    letter-spacing: 1px;
    color: #002817;
    margin-top: 5rem;
}
.line-about {
    width: 83px;
    height: 6px;
    background: #08804b;
}
.text-edit {
    font-style: normal;
    font-weight: normal;
    font-size: 24px;
    line-height: 30px;
    color: #002817;
}
.vision {
    background: rgba(0, 58, 33, 0.07);
    padding: 3rem 0 3rem 0;
}
.vision-text {
    font-style: normal;
    font-weight: bold;
    font-size: 28px;
    line-height: 28px;
    letter-spacing: 1px;
    color: #002817;
    text-align: center;
}
.line-2 {
    width: 83px;
    height: 6px;
    background: #08804b;
    margin: auto;
}
.break::after {
    content: "\a";
    white-space: pre;
}
@media screen and (max-width: 768px) {
    .about-header {
        margin-top: 1rem;
    }
}
@media screen and (max-width: 1024px) {
    .style-container {
        margin: 1rem;
    }
    .about-header {
        margin-top: 1rem;
    }
}
</style>