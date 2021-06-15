<template>
  <section>
    <IconElement
      :data="data.first"
      name="projects"
    />
    <IconElement
      :data="data.second"
      name="users"
    />
    <IconElement
      :data="data.third"
      name="postedMonthly"
    />
  </section>
</template>

<script>
import IconElement from '@/components/Home/IconSection/IconElement.vue';

export default {
  props: {
    data: Object,
  },
  name: 'IconSection',
  components: { IconElement },
};
</script>

<style scoped lang="scss">
section {
  margin-top: 128px;
  padding: 96px 0;
  background-color: $tertiary-color;
}
</style>
