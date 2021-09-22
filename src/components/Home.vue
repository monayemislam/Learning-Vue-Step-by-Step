<template>
    <div>
        <h2>Checkbox and Radio Button</h2>

        <h4>Which programming language want to learn?</h4>

        <label>PHP</label>
        <input type="checkbox" v-model="languages" id="php" value="Php">

        <label>Java</label>
        <input type="checkbox" v-model="languages" id="java" value="Java">
        <label>Python</label>
        <input type="checkbox" v-model="languages" id="python" value="Pythod">

        <h4>Selected Languages: {{languages}}</h4>
    </div>
    <div>

        <h4>Select Role</h4>
        <label>IoT Engineer</label>
        <input type="radio" v-model="srole" id="iot" value="IoT Engineer" name="profession">
        <label>Data Scientist</label>
        <input type="radio" v-model="srole" id="data" value="Data Scientist" name="profession">

        <h4>Selected Role: {{srole}}</h4>
    </div>
</template>

<script>
    export default{
        name: "Home",
        data()
        {
            return{
               languages: [],
               srole: null
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