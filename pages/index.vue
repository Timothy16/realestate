<template>
    <div>
        <hero-section />
        <home-section />
        <rent-section />
        <cities />
        <border-line />
        <property-managment />
    </div>
</template>

<script>
export default {
    data(){
        return{
            stuff:{ }
        }
    },
    mounted(){
        this.getStuff()
    },
    methods:{
        getStuff(){
        this.$axios.get("https://api.jayceeandjay.com/rents", {headers : {'Content-Type':'application/json'}}).then((res)=> {
               this.stuff=res.data;
               console.log(this.stuff)
         }) 
    },
}
};

</script>

<style scoped>
</style>