<template>
    <div>
        <div class="container">
            <div class="grid mb-5">
                <div class="four"></div>
                <div class="one">
                    <div class="two">
                        <h1>Login</h1>
                        <div class="three">
                            <form action="" @submit.prevent="login">
                                <input
                                type="email"
                                placeholder="Email Address"
                                v-model="loginInfo.email"
                            />
                            <input type="password" placeholder="Password" 
                            v-model="loginInfo.password"/>
                            <button type="submit">Log In</button>
                            </form>
                            
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    data(){
        return{
            loginInfo : {
                username:'',
                password : '',
                email:'',

            },
            registrationResponse:{}
             
        }
    },
    methods:{
        login(){
             this.$axios.post('https://api.jayceeandjay.com/rest-auth/login/', this.loginInfo,
              {headers : {'Content-Type':'application/json'}}).then((res)=> {
                this.registrationResponse=res.data;
               console.log(this.registrationResponse)

            })
           
        },
    }
}
</script>
<style scoped>
.grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
}
.one {
    height: 80vh;
    background: white;
    padding-left: 10vh;
    padding-right: 10vh;
}
.two {
    padding-top: 10vh;
}
.two h1 {
    color: #00321c;
    font-size: 48px;
    margin-bottom: 5vh;
}
.two p {
    color: #08804b;
    font-size: 24px;
    margin-top: -1vh;
}
.three input {
    display: block;
    margin-bottom: 3vh;
    width: 100%;
    background: #eff0f7;
    border-radius: 10px;
    border: none;
    padding-left: 1vh;
    padding-top: 1vh;
    padding-bottom: 1vh;
    border: 1px solid #00321c;
}
.three button {
    margin-bottom: 2vh;
    margin-top: 5vh;
    width: 100%;
    border-radius: 10px;
    color: white;
    background: #08804b;
    border: none;
    padding-top: 1.5vh;
    padding-bottom: 1.5vh;
    font-size: 3vh;
}
.four {
    background: linear-gradient(
            to right,
            rgba(0, 4, 23, 0.58),
            rgba(0, 4, 23, 0.58)
        ),
        url("/img/hero/hero.png");
    height: auto;
    background-size: cover;
    background-position: center;
}

@media (max-width: 578px) {
    .two h1 {
        color: white;
        font-size: 48px;
    }
    .two p {
        color: white;
        font-size: 20px;
        margin-top: -1vh;
    }
    .four {
        display: none;
    }
    .grid {
        display: grid;
        grid-template-columns: 1fr;
    }
    .one {
        height: 80vh;
        background: linear-gradient(
                to right,
                rgba(0, 4, 23, 0.58),
                rgba(0, 4, 23, 0.58)
            ),
            url("/img/hero/hero.png");
        background-size: cover;
        background-position: center;
        padding-left: 3vh;
        padding-right: 3vh;
    }
    label {
        color: white;
    }
}
.three button {
    margin-bottom: 3vh;
    margin-top: 5vh;
    width: 100%;
    border-radius: 10px;
    color: white;
    background: #08804b;
    border: none;
    padding-top: 1.5vh;
    padding-bottom: 1.5vh;
    font-size: 3vh;
}

@media (min-width: 579px) and (max-width: 769px) {
    .one {
        height: 80vh;
        padding-left: 3vh;
        padding-right: 3vh;
    }
}
@media (min-width: 770px) and (max-width: 1200px) {
    .one {
        height: 80vh;
        padding-left: 3vh;
        padding-right: 3vh;
    }
}
</style>