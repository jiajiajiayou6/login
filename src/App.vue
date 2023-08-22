<template>
  <div id="app">
    <nav></nav>
    <router-view />
  </div>
</template>

<style lang="less">
#app {
  width: 100%;
  height: 100vh;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-image: url("https://img0.baidu.com/it/u=1279247115,2726117336&fm=253&fmt=auto&app=138&f=JPEG?w=889&h=500");
  background-size: 100% 100%;
}

nav {
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
<style>
* {
  margin: 0;
  padding: 0;
}
li {
  list-style: none;
}
a {
  text-decoration: none;
}
</style>
