<template>
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
    margin: 7rem 5rem 7rem 8rem;
}
@media screen and (max-width: 768px) {
    .style-container {
        margin: 1rem;
    }
}
</style>