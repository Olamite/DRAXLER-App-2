# DRAXLER-App-2
DApp Fusion Dex Design

Bash

npm install -g @vue/cli
vue create draxler
cd draxler

npm install vue-router

Vue.js

draxler/
├── public/
│   ├── index.html
│   └── ...
├── src/
│   ├── assets/
│   │   └── ...
│   ├── components/
│   │   └── ...
│   ├── views/
│   │   └── ...
│   ├── App.vue
│   └── main.js
└── ...

Html

<template>
  <div id="app">
    <header>
      <!-- Header content -->
    </header>
    <router-view></router-view>
    <footer>
      <!-- Footer content -->
    </footer>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
/* Global styles */
</style>

Javascript

import Vue from 'vue'
import App from './App.vue'
import VueRouter from 'vue-router'

Vue.use(VueRouter)

const router = new VueRouter({
  routes: [
    // Define your routes here
  ]
})

new Vue({
  router,
  render: h => h(App)
}).$mount('#app')

CSS

/* Reset styles */
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

/* Global styles */
body {
  font-family: Arial, sans-serif;
  background-color: #f8f8f8;
  color: #333;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px;
}

header, footer {
  background-color: #fff;
  padding: 10px 20px;
  border-bottom: 1px solid #ddd;
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

footer {
  text-align: center;
}

nav {
  display: flex;
}

nav ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  display: flex;
}

nav ul li {
  margin-right: 20px;
}

nav ul li a {
  text-decoration: none;
  color: #333;
  font-weight: bold;
  transition: color 0.3s ease;
}

nav ul li a:hover {
  color: #007bff;
}

/* Button styles */
.btn {
  display: inline-block;
  padding: 10px 20px;
  background-color: #007bff;
  color: #fff;
  text-decoration: none;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.btn:hover {
  background-color: #0056b3;
}

/* Form styles */
.form-group {
  margin-bottom: 20px;
}

.form-group label {
  display: block;
  margin-bottom: 5px;
  font-weight: bold;
}

.form-group input[type="text"],
.form-group input[type="password"] {
  width: 100%;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 5px;
}

.form-group input[type="submit"] {
  background-color: #007bff;
  color: #fff;
  border: none;
  border-radius: 5px;
  padding: 10px 20px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.form-group input[type="submit"]:hover {
  background-color: #0056b3;
}
