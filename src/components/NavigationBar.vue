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
}

li {
  list-style: none;
  padding: 24px 0;
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

@media only screen and (max-width: 480px) {
  .navbar ul {
    justify-content: center;
  }
  li a {
    padding: 12px 10px;
    font-size: 12px;
  }
  img {
    width: 20px;
    padding: 0 0 0 24px;
  }
}
</style>
