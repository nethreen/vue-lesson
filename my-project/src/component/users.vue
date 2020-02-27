<template>
    <div>
        <h2>Computed Props</h2>
        <input type="text" v-model="name">
        <input type="text" v-model="work"> 
      
        <p>{{fullName()}}</p>

            <h2>Bind</h2>
        <a v-bind:href="links">My GitHub profile</a>
    </div>
</template>
<script>
    export default {
        name: 'users',
        data() {
            return {
                name: "Nəzrin Soltanlı",
                work: "Front-end Developer",
                links : "https://github.com/nezrin13?tab=repositories"
            }
        },

        methods: {
            fullName: function () {
                return this.name + " " + this.work
            }
        }

    }
</script>
<style>

</style>