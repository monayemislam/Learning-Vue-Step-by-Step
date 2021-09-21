<template>
    <div>
        <h1>Example of Methods</h1>
        <h4>My name is: {{userInfo().userName}}</h4>
        <h4>My Email: {{userInfo().userEmail}}</h4>
        <h4>My Age is: {{userInfo().userAge}}</h4>
    </div>
</template>

<script>
    export default{
        name: "Home",
        data()
        {
            return {
                name: "Monaem",
                email: "test@email.com"
            }
        },
        methods:{
            userInfo(){
                return {
                    userName: this.name,
                    userEmail: this.email,
                    userAge: "24"
                }
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