<template lang="pug">
  .social-media
    a(href='https://github.com/quirozcarlos' target="_blank")
      v-icon(:size="size") mdi-github
    a(href='https://www.linkedin.com/in/quirozvcarlos/' target="_blank")
      v-icon(:size="size") mdi-linkedin
    a(href='https://twitter.com/quirozvcarlos' target="_blank")
      v-icon(:size="size") mdi-twitter
    a(href='mailto:quirozvcarlos@gmail.com' target="_blank")
      v-icon(:size="size") mdi-email
</template>

<script>
export default {
  name: 'SocialMedia',

  props: {
    size: {
      type: String,
      default: '24'
    }
  }
}
</script>

<style lang="scss" scoped>
.social-media {
  display: flex;
  justify-content: space-evenly;
  max-width: 120px;
  a {
    margin-left: 5px;
    text-decoration: none;
  }
}
</style>
