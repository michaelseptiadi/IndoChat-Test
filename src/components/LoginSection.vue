<script setup></script>

<template>
  <div class="login">
    <div class="title-section">
      <p>Please log in to start using</p>
      <h4>Booked Tool</h4>
    </div>
    <div class="form-section">
      <input type="text" placeholder="Email" />
      <input type="password" placeholder="Password" />
      <button>Login</button>
    </div>
  </div>
</template>

<style scoped>
.login {
  margin-top: -5px;
  padding: 48px;
  height: fit-content;
  background-color: rgb(239, 239, 239);
  display: flex;
  justify-content: center;
  align-items: center;
}

.title-section h4 {
  font-size: 24px;
  font-weight: bolder;
  letter-spacing: 0.2em;
}

.form-section {
  margin-left: 48px;
}

input {
  height: 36px;
  width: 200px;
  font-size: 16px;
  border: none;
  border-radius: 4px;
  margin: 0 20px;
  padding: 8px;
}

input:focus {
  border: none;
}

@media only screen and (max-width: 950px) {
  .login,
  .form-section {
    display: flex;
    flex-direction: column;
    /* align-items: center;
    justify-content: center; */
  }
  .title-section {
    text-align: center;
  }
  input {
    height: 36px;
    width: 300px;
    font-size: 16px;
    border: none;
    border-radius: 4px;
    margin: 8px 20px;
    padding: 8px;
  }
}
</style>
