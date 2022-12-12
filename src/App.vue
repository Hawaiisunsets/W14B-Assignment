<template>
  <div id="app">
    <router-link to="/">Home</router-link>
    <router-link to="/game">Game</router-link>
    <LoginApp/>
    <GameScreen/>
    <router-view/>
  </div>
</template>

<script>
import LoginApp from "@/components/LoginApp.vue";
import GameScreen from "@/components/GameScreen.vue";
export default{
  name : "App",
  components : {
    LoginApp,
    GameScreen,
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
html{
  background-color: bisque;
}
</style>
