<template>
  <div id="app">
    <el-menu
      default-active = "4"
      class="el-menu-demo"
      mode="horizontal"
      background-color="#3498db"
      text-color="#ffffff"
      active-text-color="#ffffff"
    >
      <el-menu-item index="1">
        <router-link :to="{ path: '/'}">Home</router-link>
      </el-menu-item>
      <el-menu-item index="2">
        <router-link :to="{ path: '/todo-list'}">Todo List</router-link>
      </el-menu-item>
      <el-menu-item index="3">
        <router-link :to="{ path: '/issue-list'}">Issues</router-link>
      </el-menu-item>
      <el-menu-item index="4">
        <router-link :to="{ path: 'todo-issues'}">Todo Issues</router-link>
      </el-menu-item>
    </el-menu>

    <router-view />
  </div>
</template>

<script>


</script>

<style>
* {
  margin: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}

.el-menu-demo {
  margin-bottom: 20px;
}
.el-menu-item a,
.el-menu-item a:hover,
.el-menu-item a:active,
.el-menu-item a:focus {
  text-decoration: none;
}
</style>
