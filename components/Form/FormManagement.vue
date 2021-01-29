<template>
    <div class="form-edit">
        <div class="form-head">PROPERTY MANAGEMENT</div>
        <p>
            Please message us with your details & requirements, and we will get in touch,
            to satisfy your every property maintenance/ service need!!!
        </p>
        <form action="" @submit.prevent="messages">
            <div>
                <input
                    type="text"
                    class="form-control input"
                    placeholder="Full Name"
                    required
                    v-model="messageInfo.name"
                />
            </div>
            <div class="mt-1">
                <input
                    type="email"
                    class="form-control input"
                    placeholder="Email Address"
                    required
                    v-model="messageInfo.email"
                />
            </div>
            <div class="mt-1">
                <textarea name="" 
                id="" 
                class="form-control input" 
                placeholder="Message"
                required
                v-model="messageInfo.context"
                ></textarea>
            </div>
            <button class="btn btn-send mt-4" type="submit">Message Us</button>
        </form>
    </div>
</template>
<script>
import ElementUI from 'element-ui';
import 'element-ui/lib/theme-chalk/index.css';
export default {
    
    data(){
        return{
            salesItems:{},
            messageResponse:{},
            messageInfo : {
                name:'',
                email : '',
                context : '',
            },
        }
    },
    mounted(){
        this.searchSalesItems()
    },
    methods:{
    searchSalesItems(){
        this.$axios.get("https://api.jayceeandjay.com/salesearch", {headers : {'Content-Type':'application/json'}}).then((res)=> {
               this.salesItems=res.data.results;
               console.log(this.salesItems)
         }) 
    },
    messages(){
             this.$axios.post('https://api.jayceeandjay.com/propertymanagement/', this.messageInfo,
              {headers : {'Content-Type':'application/json'}}).then((res)=> {
                  
                this.messageResponse=res.data;

               console.log(this.messageResponse);
               this.$message({
            message:"Message Sent!",
            type: "success",
          });this.messageInfo={};

            }).catch((error) => {
          console.log(error);
        
        });
           
        },
}
};

</script>
<style scoped>
.form-edit {
    padding: 1rem 0 0 0;
}
.form-head {
    font-style: normal;
    font-weight: bold;
    font-size: 28px;
    line-height: 28px;
    letter-spacing: 0.03em;
    text-transform: uppercase;
    color: #002817;
    margin-bottom: 1rem;
}
label {
    color: #002817;
    font-style: normal;
    font-weight: bold;
}
input {
    background: #eff0f7;
    width: 70%;
    margin-bottom: 1.5rem;
}
textarea {
    background: #eff0f7;
    width: 70%;
}
.btn-send {
    background: #08804b;
    border-radius: 6px;
    text-align: center;
    color: #fff;
    width: 70%;
}

@media screen and (max-width: 768px) {
    .form-edit {
        padding: 1rem;
    }
    input {
        width: 100%;
    }
    textarea {
        width: 100%;
    }
    .btn-send {
        width: 100%;
    }
    .form-head {
        font-style: normal;
        font-weight: bold;
        font-size: 18px;
        line-height: 28px;
        letter-spacing: 0.03em;
        text-transform: uppercase;
        color: #002817;
        margin-top: 1rem;
    }
}
@media screen and (min-width: 1000px) and (max-width: 1024px) {
    .form-edit {
        padding: 0;
    }
}
</style>