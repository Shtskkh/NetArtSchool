<script setup>

</script>

<template>
<div class="login">
  <div class="login__container">
    <h3 class="login__title">Вход</h3>
    <input class="input login__email" type="email" placeholder="Email или логин">
    <input class="input login__password" type="password" placeholder="Пароль">
    <button class="btn-primary login__button">Войти</button>
    <router-link class="login__link" to="/reset">Не можете войти?</router-link>
  </div>
</div>
</template>

<style scoped>

.login {
  min-height: 100vh;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.login__container {
  display: flex;
  flex-direction: column;
  padding: 32px 16px;
  border: 2px solid var(--main-color);
  border-radius: 8px;
}

.login__title {
  text-align: center;
  margin-bottom: 32px;
}

.input {
  display: inline-block;
  height: 56px;
  padding: 16px 20px;
}

.login__email {
  margin-bottom: 16px;
}

.login__password {
  margin-bottom: 32px;
}

.login__button {
  height: 56px;
  font-size: 20px;
  margin-bottom: 16px;
}

@media (min-width: 1280px) {
  .login__container {
    width: 400px;
  }
}
@media (min-width: 640px) and (max-width: 1279px) {
  .login__container {
    width: 400px;
  }
}
@media (max-width: 639px) {
  .login__container {
    width: 360px;
  }
}

</style>