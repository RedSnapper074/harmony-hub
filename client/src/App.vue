<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>


<style>
#app {
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e40;
    background-color: #f0f0f0;
}

.register {
    width: 100%;
    background-color: #292929;
}

.register img {
    margin-top: 10px;
    width: 200px;
    background-color: green;
    border-radius: 50px;
    padding: 10px;
}

.register input{
    width: 400px;
    height: 40px;
    padding-left: 10px;
    display: block;
    margin-bottom: 20px;
    margin-left: auto;
    margin-right: auto;
    border: 1px solid green;
    border-radius: 20px;
}

.register button {
    width: 320px;
    padding: 10px;
    background: lightgreen;
    border-radius: 50px;
    border: 1px solid green;
    cursor: pointer; 
    margin-bottom: 30px
}

h1 {
    color: green;
    font-size: 60px;
}
</style>
