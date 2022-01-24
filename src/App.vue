<template>
  <div id="app">
    <div class="nav-bar">
      <span class="nav-bar-contents" @click="$router.push('/')">Home</span>
      <span class="nav-bar-contents" @click="$router.push('/about')">About</span>
    </div>
    <router-view/>
  </div>
</template>

<style>
html, body, #app {
  width: 100%;
  height: 100%;
}
body {
  margin: 0;
  background-color: #262626;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

.nav-bar {
  padding: 30px 40px;
  text-align: center;
}

.nav-bar-contents {
  color: #f1f1f1;
  font-size: 20px;
  font-weight: 800;
  margin: 0 10px 0 10px;
  border: none !important;
  cursor: pointer;
}

.nav-bar-contents:hover {
  color: #3fccf7;
}
</style>
