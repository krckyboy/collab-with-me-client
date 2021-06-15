<template>
  <header class="header">
    <router-link class="section section--left" to="/">
      <img src="@/assets/logo.svg" alt="logo" class="logo">
    </router-link>
    <div class="section section--right">
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

<style lang="scss" scoped>
header {
  padding: 8px 24px;

  &, .section--right {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .logo {
    width: 48px;
    height: 48px;
  }

  .section--right {
    a {
      font-weight: bold;
    }

    .register {
      border-radius: 12px;
      border: 3px solid $secondary-color;
      color: $secondary-color;
      padding: 12px;
      margin-left: 24px;
    }
  }
}

.router-link-exact-active {
  font-weight: bold;
}
</style>
