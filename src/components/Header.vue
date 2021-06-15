<template>
  <header class="header">
    <router-link class="header__section header__section--left" to="/">
      <img src="@/assets/logo.svg" alt="logo" class="logo">
    </router-link>
    <div class="header__section header__section--right">
      <router-link class="login" to="/login">Login</router-link>
      <router-link class="register" to="/register">Register</router-link>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
};
</script>

<style lang="scss">
.header {
  padding: 8px 24px;

  &, &__section--right {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  &__logo {
    width: 48px;
    height: 48px;

    img {
      width: 100%;
    }
  }
}

.router-link-exact-active {
  font-weight: bold;
}
</style>
