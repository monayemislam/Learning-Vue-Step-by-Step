<template>
    <div>
        <h2>Example of Two way Binding</h2>
        <h4>Please Enter a value</h4>
        <input type="text" v-model="value">
        <h4>You have entered: {{value}}</h4>
    </div>
</template>

<script>
    export default{
        name: "Home",
        data()
        {
            return{
                value: 0
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