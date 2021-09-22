<template>
    <div>
        <h2>Conditional Rendering (IF-Else)</h2>
        <h4 v-if="show">Hi ! I am the if condition</h4>
        <h4 v-else>Else condition</h4>
        <button v-on:click="show=!show">Click Me For Toggle</button>
    </div>
</template>

<script>
    export default{
        name: "Home",
        data()
        {
            return{
               show: true
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