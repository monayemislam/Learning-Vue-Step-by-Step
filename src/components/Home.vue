<template>
    <div>
        <h4>Count: {{count}}</h4>
        <button v-on:click="increaseCount()">Increase</button>
        <button v-on:click="decreaseCount()">Decrease</button>
    </div>
</template>

<script>
    export default{
        name: "Home",
        data()
        {
            return{
                count: 0
            }
        },
        methods:{
            increaseCount(){
               this.count = this.count+1;
            },
            decreaseCount(){
               this.count = this.count-1;
            }
        }
    }
</script>

<style scoped>
    div{
        color: skyblue;
        border: 2px solid skyblue;
    }
</style>