<template>
  <div id="nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/glav">glav</router-link>
    <router-link to="/Conect">Conect</router-link>
    <router-link to="/Contacts">Contacts</router-link>
    <router-link to="/GlavCard">GlavCard</router-link>
    <router-link to="/Your">Your</router-link>
    <router-link to="/All">All</router-link>
    <router-link to="/Item">Item</router-link>
    <router-link to="/Buy">Buy</router-link>
  </div>
  <router-view />
</template>

<style scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  flex-wrap: wrap;
}
#nav a.router-link-exact-active {
  color: #42b983;
}
</style>

