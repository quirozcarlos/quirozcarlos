<template lang="pug">
  v-parallax(height='500' src='https://cdn.vuetifyjs.com/images/parallax/material.jpg')
    v-row(align='center' justify='center')
      v-col.text-center(cols='12')
        h1.display-1.font-weight-thin.mb-4
          | Hi 👋
</template>

<script>
export default {
  name: 'Index',
  components: {}
}
</script>
