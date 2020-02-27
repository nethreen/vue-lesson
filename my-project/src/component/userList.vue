<template>
    <div id="userlist">
        <p>Ad: {{firstName}}</p>
        <p>Soyad: {{lastName}} </p>
        <p>Address: {{address}} </p>
        <p> {{myFullName()}}</p>


    </div>
</template> 

<script>
export default {
  name: 'userList',
  data () {
    return {
        firstName : "Nəzrin",
        lastName : "Soltanlı",
        address : "Bakı"
    }
  },
  methods: {

    myFullName: function(){
        return "Uğurlar" + " " + this.firstName + " " + this.lastName + " " ;
    }
  }
}
</script>
<style>
    
</style>