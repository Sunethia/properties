<template>
  <nav>
    <li><router-link to="/home">Home</router-link></li>
    <router-link to="/about">About</router-link>
    <router-link to="/properties">Properties</router-link>
    <router-link to="/admin">Admin</router-link>
  </nav>
</template>
<script>
export default {};
</script>
<style>
nav {
  display: flex;
  align-items: center;
  justify-content: space-evenly;
  padding: 30px;
  background-color: rgb(237, 246, 249);
}
nav a {
  font-weight: bold;
  color: rgb(0, 109, 119);
}
</style>
