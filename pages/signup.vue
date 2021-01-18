<template>
    <div>
        <div>
            <div class="grid">
                <div class="four">

                </div>
                <div class="one">
                    <div class="two">
                        <h1>Create Account</h1>
                    <p>To make an enquiry</p>
                    <div class="three">
                        <label for="">Name</label>
                        <input type="text" placeholder="John Doe">
                        <label for="">Phone Number</label>
                        <input type="Number" placeholder="0123456789">
                        <label for="">Email Address</label>
                        <input type="email" placeholder="johndoe@gmail.com">
                        <label for="">Password</label>
                        <input type="password" placeholder="*******">
                        <button type="submit">Submit</button>
                    </div>
                    </div>
                    
                </div>
            </div>
        </div>
    </div>
</template>
<style scoped>
    .grid{
        display: grid;
        grid-template-columns: 1fr 1fr;
    }
    .one{
        height: 100vh;
        background: white;
        padding-left: 10vh;
        padding-right: 10vh;
    }
    .two{
        padding-top: 5vh;
    }
    .two h1{
        color: #00321C;
        font-size: 48px;
    }
    .two p{
        color: #08804B;
        font-size: 24px;
        margin-top: -1vh;
    }
    .three input{
        display: block;
        margin-bottom: 2vh;
        width: 100%;
        background: #EFF0F7;
        border-radius: 10px;
        border: none;
        padding-left: 1vh;
        padding-top: 1vh;
        padding-bottom: 1vh;
        border: 2px solid #14142B;
    }
    .three button{
        margin-bottom: 2vh;
        margin-top: 5vh;
        width: 100%;
        border-radius: 10px;
        color: white;
        background: #08804B;
        border: none;
        padding-top: 1.5vh;
        padding-bottom: 1.5vh;
        font-size: 3vh;
    }
    .four{
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



    @media(max-width:578px){
        .two h1{
        color: white;
        font-size: 48px;
    }
    .two p{
        color: white;
        font-size: 20px;
        margin-top: -1vh;
    }
    .four{
        display: none;
    }
    .grid{
        display: grid;
        grid-template-columns: 1fr;
    }
     .one{
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
        label{
            color: white;
        }
    }
     .three button{
        margin-bottom: 3vh;
        margin-top: 5vh;
        width: 100%;
        border-radius: 10px;
        color: white;
        background: #08804B;
        border: none;
        padding-top: 1.5vh;
        padding-bottom: 1.5vh;
        font-size: 3vh;
    }
    


    @media(min-width:579px) and (max-width:769px){
        .one{
        height: 100vh;
        padding-left: 3vh;
        padding-right: 3vh;
    }
        
    }
    @media(min-width:770px) and (max-width:1200px){
        .one{
        height: 100vh;
        padding-left: 3vh;
        padding-right: 3vh;
    }
        
    }
</style>