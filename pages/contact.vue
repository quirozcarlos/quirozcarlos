<template lang="pug">
  v-row(align='center' justify='center')
    v-col.text-center(cols='12')
      h3.title.font-weight-thin
        | If you have any questions about my services, or just want to say hello, feel free to contact me. Below are my social pages and my email:
      .d-flex.justify-center
        social-media(size="50")
</template>

<script>
import SocialMedia from '@/components/utils/SocialMedia'
export default {
  name: 'Contact',

  components: {
    SocialMedia
  }
}
</script>

<style lang="scss" scoped>
.title {
  font-size: 24px;
  margin: 0 50px 50px;
}

</style>
