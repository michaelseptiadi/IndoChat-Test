<script setup></script>

<template>
  <div class="navbar">
    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#discover">Discover</a></li>
      <li><a href="#register">Register</a></li>
      <li><img src="../assets/search.svg" /></li>
    </ul>
  </div>
</template>

<style scoped>
.navbar {
  background-color: rgb(239, 239, 239);
  width: 100%;
  height: 70px;
  z-index: 1;
}

.navbar ul {
  display: flex;
  justify-content: flex-end;
  margin-right: 50px;
}

li {
  list-style: none;
  padding: 28px 0;
}

li a {
  text-decoration: none;
  color: rgb(40, 40, 40);
  padding: 12px 36px;
  border-radius: 24px;
}

li a:hover,
li a:focus {
  background-color: rgb(198, 198, 198);
}

img {
  width: 20px;
  padding: 0 36px;
}
</style>
