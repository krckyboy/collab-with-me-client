<template>
  <div class="home section-padding">
    <IllustrationSection
      title="Looking for project based gigs?"
      text="Fill up your profile and you’re ready. Find a project that you like and apply.
        People post all kinds of projects, paid or not, remote or location based, so you’ll
        probably find something nice here!"
      buttonText="Find Projects"
      imageName="illustration-1.svg"
    />
    <IllustrationSection
      title="Need to find people for the project?"
      text="Create a project, fill up all the fields and wait for users to apply
        or you can let them know that you find them suitable for the job!"
      buttonText="Find People"
      imageName="illustration-2.svg"
    />
  </div>
</template>

<script>

import IllustrationSection from '@/components/IllustrationSection.vue';

export default {
  name: 'Home',
  components: {
    IllustrationSection,
  },
};
</script>
