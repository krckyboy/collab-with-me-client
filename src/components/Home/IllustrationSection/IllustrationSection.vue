<template>
  <section class="section-padding">
    <illustration
      :data="data.first"
    />
    <illustration
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
