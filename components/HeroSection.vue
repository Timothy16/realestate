<template>
    <div>
        <div class="wrapper">
            <div class="container">
                <div class="wrapper-content hello">
                    <div class="header-title">home at last</div>
                    <div class="header-text">
                        Your Home Realtors you can trust
                    </div>
                    <!-- <div class="button-edit">
                        <div class="">
                            <div>
                                <nuxt-link to="/search_buy">
                                    <div class="btn btn-buy">BUY</div>
                                </nuxt-link>
                                <nuxt-link to="/search_rent"
                                    ><div class="btn btn-rent">RENT</div>
                                </nuxt-link>
                            </div>
                        </div>
                    </div> -->
                    <!-- <div class="search-session rounded">
                        <div class="d-flex">
                            <span style="margin-top: 0.6rem"
                                ><font-awesome-icon :icon="['fa', 'search']"
                            /></span>
                            <input
                                class="pl-3"
                                type="text"
                                placeholder="Search City, Street,Apartment"
                            />
                        </div>
                        <div class="stroke">|</div>
                        <hr class="line-on-mobile" />
                        <div class="top-down">
                            <select class="" id="options">
                                <option selected disabled>Rooms</option>
                                <option>2</option>
                                <option>3</option>
                                <option>4</option>
                            </select>
                        </div>
                        <div class="stroke">|</div>
                        <hr class="line-on-mobile" />
                        <div class="top-down">
                            <select class="" id="options">
                                <option selected disabled>State</option>
                                <option>2</option>
                            </select>
                        </div>
                        <div class="btn btn-search top-down">Search</div>
                    </div> -->
                    <!-- <div class="angle-edit">
                        <font-awesome-icon
                            :icon="['fa', 'angle-double-down']"
                        />
                    </div> -->
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
.wrapper {
    background: linear-gradient(
            to right,
            rgba(0, 4, 23, 0.58),
            rgba(0, 4, 23, 0.58)
        ),
        url("/img/hero/hero.png");
    height: auto;
    padding-bottom: 1rem;
    background-size: cover;
    background-position: center;
}
.wrapper-content {
    margin: auto;
    width: 70%;
    padding-top: 20rem;
    padding-bottom: 10rem;
}
.header-title {
    font-style: normal;
    font-weight: bold;
    font-size: 64px;
    line-height: 58px;
    text-align: center;
    letter-spacing: 0.02em;
    color: #ffffff;
    /* text-shadow: 4px 4px 7px rgba(0, 0, 0, 0.25); */
    /* backdrop-filter: blur(44px); */
    text-transform: uppercase;
}
.header-text {
    font-style: normal;
    font-weight: normal;
    font-size: 24px;
    line-height: 35px;
    text-align: center;
    letter-spacing: 0.02em;
    color: #c9c9c9;
    margin-top: 1rem;
}
.button-edit {
    display: flex;
    text-align: center;
    justify-content: center;
    align-items: center;
    margin-top: 2rem;
}
.btn-buy {
    background: #08804b;
    border-radius: 4px 0px 0px 4px;
    color: #fff;
    padding-left: 3rem;
    padding-right: 3rem;
}
.btn-rent {
    background: #ffffff;
    border-radius: 0px 4px 4px 0px;
    color: #08804b;
    padding-left: 3rem;
    padding-right: 3rem;
    position: relative;
    left: -4px;
}
.search-session {
    background: #fff;
    padding: 1rem;
    display: flex;
    justify-content: space-between;
    margin-top: 2rem;
}
::placeholder {
    font-style: normal;
    font-weight: normal;
    font-size: 12px;
    line-height: 22px;
    text-align: center;
    letter-spacing: 0.06em;
    color: #afafaf;
    margin-right: 0.5rem;
}
input {
    outline: none;
    border: none;
    width: 100%;
}
select {
    outline: none;
    border: none;
    width: 100%;
    padding: 0.5rem;
    color: #afafaf;
}
.stroke {
    color: #c4c4c4;
    margin-top: 0.5rem;
}
option {
    font-style: normal;
    font-weight: normal;
    font-size: 15px;
    line-height: 22px;
    text-align: center;
    letter-spacing: 0.06em;
    color: #afafaf;
}
.btn-search {
    background: #08804b;
    border-radius: 8px;
    color: #fff;
    padding-right: 3rem;
    padding-left: 3rem;
    /* width: 100%; */
}
.angle-edit {
    color: #fff;
    text-align: center;
    font-size: 24px;
    margin-top: 3rem;
    cursor: pointer;
}
.line-on-mobile {
    display: none;
}
@media screen and (max-width: 578px) {
    .wrapper {
        background: linear-gradient(
                to right,
                rgba(0, 4, 23, 0.58),
                rgba(0, 4, 23, 0.58)
            ),
            url("/img/hero/hero.png");
        height: auto;
        padding-bottom: 1rem;
        background-size: cover;
        background-position: center;
    }
    .wrapper-content {
        margin: auto;
        width: 100%;
        padding-top: 2rem;
         padding-bottom: 2rem;
    }
    .header-title {
        font-style: normal;
        font-weight: bold;
        font-size: 24px;
        line-height: 58px;
        text-align: center;
        letter-spacing: 0.02em;
        color: #ffffff;
        /* text-shadow: 4px 4px 7px rgba(0, 0, 0, 0.25); */
        /* backdrop-filter: blur(44px); */
        text-transform: uppercase;
    }
    .header-text {
        font-style: normal;
        font-weight: normal;
        font-size: 16px;
        line-height: 35px;
        text-align: center;
        letter-spacing: 0.02em;
        color: #c9c9c9;
        margin-top: 0.2rem;
    }
    .search-session {
        padding: 1rem;
        display: block;
        margin-top: 1rem;
    }
    .stroke {
        display: none;
    }
    .btn-search {
        width: 100%;
    }
    .top-down {
        margin-top: 0.5rem;
    }
    .line-on-mobile {
        display: block;
        color: #afafaf;
    }
    .button-edit {
        margin-top: 1rem;
    }
}
@media screen and (min-width: 710px) and (max-width: 1024px) {
    .wrapper-content {
        margin: auto;
        width: 100%;
        padding-top: 16rem;
    }
    .wrapper {
        background: linear-gradient(
                to right,
                rgba(0, 4, 23, 0.58),
                rgba(0, 4, 23, 0.58)
            ),
            url("/img/hero/hero.png");
        height: auto;
        padding-bottom: 1rem;
        background-size: cover;
        background-position: center;
    }
}
</style>