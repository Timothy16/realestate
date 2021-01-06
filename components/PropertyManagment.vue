<template>
    <div>
        <div class="style-container">
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
.style-container {
    margin: 7rem 5rem 7rem 8rem;
}
@media screen and (max-width: 768px) {
    .style-container {
        margin: 1rem;
    }
}
@media screen and (min-width: 1000px) and (max-width: 1024px) {
    .style-container {
        margin: 1rem;
    }
    .card {
        width: 100%;
    }
}
</style>