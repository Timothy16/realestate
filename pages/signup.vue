<template>
    <div>
        <div class="container mt-5">
            <div class="grid mb-5">
                <div class="four"></div>
                <div class="one">
                    <div class="two mt-3">
                        <h1>Create Account</h1>
                        <p>To make an enquiry</p>
                        <div class="three">
                            <form action="" @submit.prevent="register">
                                <input type="text" placeholder="Username" v-model="loginInfo.username" />
                            <input type="text" placeholder="First Name" v-model="loginInfo.first_name" />
                            <input type="text" placeholder=" Last Name" v-model="loginInfo.last_name" />
                            <input
                                type="email"
                                placeholder="Email"
                                v-model="loginInfo.email"
                            />
                            <input type="password" placeholder="Password" v-model="loginInfo.password"/>
                            <input type="password" placeholder="Verify Password" v-model="loginInfo.verify_password"/>
                            <button type="submit">Create Account</button>
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
                first_name : '',
                last_name : '',
                password : '',
                email:'',
                verify_password:'',

            },
            registrationResponse:{}
             
        }
    },
    methods:{
        register(){
             this.$axios.post('https://api.jayceeandjay.com/accounts/register/', this.loginInfo,
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
    height: 100vh;
    background: white;
    padding-left: 10vh;
    padding-right: 10vh;
}
.two {
    padding-top: 5vh;
}
.two h1 {
    color: #00321c;
    font-size: 48px;
}
.two p {
    color: #08804b;
    font-size: 24px;
    margin-top: -1vh;
    margin-bottom: 2rem;
}
.three input {
    display: block;
    margin-bottom:3vh;
    width: 100%;
    background: #eff0f7;
    border-radius: 10px;
    border: none;
    padding-left: 1vh;
    padding-top: 1vh;
    padding-bottom:1vh;
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
        height: 110vh;
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
        height: 100vh;
        padding-left: 3vh;
        padding-right: 3vh;
    }
}
@media (min-width: 770px) and (max-width: 1200px) {
    .one {
        height: 100vh;
        padding-left: 3vh;
        padding-right: 3vh;
    }
}
</style>