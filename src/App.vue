<script setup>
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>
  <header>
      <nav>
        <RouterLink to="/">Loja</RouterLink> |
        <RouterLink to="/about">Carrinho (0)</RouterLink>
      </nav>
  </header>
  <RouterView />
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  max-width: 1280px;
  margin: 80px auto;
}

nav {
  background-color: rgb(37,37,37);
  padding: 16px 0;
  position: fixed;
  z-index: 1;
  top: 0;
  left: 0;
  width: 100%;
  text-align: center;
  color: aliceblue;

  a {
    text-decoration: none;
    color: white;

    &.router-link-exact-active {
      color: #007bff;
    }
  }
  @media (hover: hover) {
  a:hover {
    background-color: hsla(160, 100%, 37%, 0.2);
  }
}
}
</style>
