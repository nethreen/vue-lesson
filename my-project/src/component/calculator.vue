<template>
    <div>
        kilometr
        <input type="text" v-model="kilometres">
        <br>
        <br>
        metr
        <input type="text" v-model="metres">
    </div>
</template>
<script>
    export default {
        name: "Calculator",
        data() {
            return {
                kilometres: 0,
                metres: 0,
            }
        },
        watch: {
            kilometres: function(data){
                this.kilometres = data;
                this.metres = data * 1000
            },
             metres: function(data){
                this.kilometres = data / 1000;
                this.metres = data;
            }
        },
    }
</script>
<style>

</style>