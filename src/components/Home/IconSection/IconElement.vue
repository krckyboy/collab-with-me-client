<template>
  <div :class="name">
    <img :src="require('@/assets/' + data.imageName + '')"
         :alt="data.label">
    <span class="value">35313</span>
    <span class="label">{{ data.label }}</span>
  </div>
</template>

<script>
export default {
  name: 'IconElement',
  props: {
    data: Object,
    name: String,
  },
};
</script>

<style scoped lang="scss">
div {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  font-weight: bold;

  &:not(:first-of-type) {
    margin-top: 64px;
  }

  &.projects {
    color: #35CC61;
  }

  &.users {
    color: #EB5757;
  }

  &.postedMonthly {
    color: #56CCF2;
  }

  img {
    width: 72px;
  }

  .value {
    font-size: 32px;
    margin-top: 15px;
    margin-bottom: 8px;
  }

  .label {
    font-size: 16px;
  }
}
</style>
