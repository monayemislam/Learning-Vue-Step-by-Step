<template>
    <div>
        <h2>Loop</h2>
        <ul>
            <li v-for="item in users" :key="item.id">
                {{item.role}} role is playing by : {{item.name}}<br>
            </li>
        </ul>
    </div>
</template>

<script>
    export default{
        name: "Home",
        data()
        {
            return{
               users:[
                   {
                       id: 12,
                       name: "Monayem",
                       role: "Web Developer"
                   },
                   {
                       id: 13,
                       name: "Shemanto",
                       role: "SEO Expert"
                   },
                   {
                       id: 14,
                       name: "Raju",
                       role: "Graphics Designer"
                   }
               ]
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