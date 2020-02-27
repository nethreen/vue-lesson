<template>
  <div id="app">
    <h2>Component</h2>
    <UserList></UserList>
    <Users></Users>
    <h2>Watch Property</h2>
    <calculator> </calculator>
    <h2>Collect</h2>
    <collect></collect>
  </div>

</template>

<script>
  import UserList from './component/userList';
  import Users from './component/users';
  import Calculator from './component/calculator';
  import Collect from './component/collect';
  export default {
    name: 'app',
    data() {
      return {
        msg: 'Xoş gəldin səhifəmə'
      }
    },

    components: {
      "UserList": UserList,
      "Users": Users,
      "Calculator": Calculator,
      "Collect" : Collect
    }
  }
</script>


<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }

  h1,
  h2 {
    font-weight: normal;
  }

  h2 {
    color: orange;
  }

  ul {
    list-style-type: none;
    padding: 0;
  }

  li {
    display: inline-block;
    margin: 0 10px;
  }

  a {
    color: #42b983;
  }
</style>