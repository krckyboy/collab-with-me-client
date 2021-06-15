<template>
  <section class="section-padding">
    <Illustration
      :data="data.first"
    />
    <Illustration
      :data="data.second"
    />
  </section>
</template>

<script>
import Illustration from '@/components/Home/IllustrationSection/Illustration.vue';

export default {
  name: 'IllustrationSection',
  props: {
    data: Object,
  },
  components: {
    Illustration,
  },
};
</script>

<style scoped>

</style>
