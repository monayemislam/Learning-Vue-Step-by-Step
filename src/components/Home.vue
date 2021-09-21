<template>
    <div>
        <h1>Example of InterPolation and Data</h1>
        <h3>{{myName}}</h3>
        <h3>{{homeTown}}</h3>
        <h3>Lenght of my name (Monayem):{{"Monayem".length}}</h3>
    </div>
</template>

<script>
    export default{
        name: "Home",
        data(){
            return {
                myName:"Monayem Islam",
                homeTown: "Chapainawabganj"
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