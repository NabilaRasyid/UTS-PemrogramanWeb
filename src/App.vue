<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header>
      <div class="wrapper">

          <nav class="navbar navbar-expand-lg fixed-top bg-body-tertiary">
              <h3 class = "title-navbar"> Al Quran </h3>
              <ul class = "nav-link">
                  <li><router-link to="/home" style="color: black"> Home </router-link></li>
                  <li><router-link to="search" style="color: black"> Search </router-link></li>
                  <li><router-link to="/surah" style="color: black"> Surah </router-link></li>
                  <li><router-link to="/ayat" style="color: black"> Ayat </router-link></li>
              </ul>
          </nav>

      </div>
  </header>

  <RouterView />
</template>

<style scoped>
.nav-link {
    background: #6d9581;
}

h3 {
    font-family: "Lucida Bright";
    padding-left: 30px;
}

li {
    font-family: "Lucida Bright";
    list-style: none;
    float: left;
    padding: 15px 30px;
    font-size: 20px;
}

</style>