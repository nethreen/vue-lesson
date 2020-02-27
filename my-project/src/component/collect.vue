<template>
    <div>
        <button v-on:click="blockNumber">Kliklə</button>
        <p>
          <input type="text" v-model="numberOne">
            <input type="text" v-model="numberTwo">

            <br>
            <br>
            Cavab {{total}}
        </p>
    </div>
</template>
<script>
export default {
    name : "Collect",
    data(){
        return{
            numberOne : 10,
            numberTwo : 10,
            total : " "
        }
    },
    methods: {
        blockNumber: function(){
            return this.total = parseInt(this.numberOne) * parseInt(this.numberTwo);
        }
    }
}
</script>
<style>

</style>