<template>
  <app-header/>
  <router-view/>
</template>

<script>
import AppHeader from '@/components/Header.vue';

export default {
  name: 'Home',
  components: {
    AppHeader,
  },
};

</script>

<style lang="scss">

</style>
