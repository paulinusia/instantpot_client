<template>
  <div id="app">
    <div id="nav">
      <router-link to="/" exact>Home</router-link>|
      <router-link to="/customers" exact>Customers</router-link>|
      <router-link to="/partners" exact>Partners</router-link>|
      <router-link to="/products" exact>Products</router-link>
    </div>
    <keep-alive>
      <router-view></router-view>
    </keep-alive>
  </div>
</template>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
