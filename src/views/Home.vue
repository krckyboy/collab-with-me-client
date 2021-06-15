<template>
  <div class="home">
    <IllustrationSection :data="illustrationSectionData"/>
    <IconSection :data="iconSectionData"/>
  </div>
</template>

<script>
import IllustrationSection from '@/components/Home/IllustrationSection/IllustrationSection.vue';
import IconSection from '@/components/Home/IconSection/IconSection.vue';
import { content } from '@/helpers/data';

export default {
  name: 'Home',
  components: {
    IllustrationSection,
    IconSection,
  },
  data() {
    const {
      illustrationSection: illustrationSectionData,
      iconSection: iconSectionData,
    } = content.home;
    return {
      illustrationSectionData,
      iconSectionData,
    };
  },
};
</script>
