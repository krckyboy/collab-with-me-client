<template>
  <section>
    <img :src="require('@/assets/' + imageName + '')"
         alt="title">
    <h1>{{ title }}</h1>
    <p>{{ text }}</p>
    <router-link to="/register" class="button button--main">{{ buttonText }}</router-link>
  </section>
</template>

<script>
export default {
  name: 'IllustrationSection',
  props: {
    title: String,
    text: String,
    buttonText: String,
    imageName: String,
  },
};
</script>

<style lang="scss" scoped>
section {
  &:first-of-type {
    margin-top: 48px;
  }

  margin-top: 148px;
}

h1 {
  font-size: 36px;
  font-weight: bold;
  margin-top: 40px;
}

p {
  font-size: 14px;
  line-height: 24px;
  margin-top: 24px;
}

.button {
  margin-top: 32px;
}

</style>
