<template lang="pug">
  v-row(align="center" justify="center" style="height: 50vh")
    v-col(align="center" cols='12')
      .wrapper
        h1.font-weight-thin.mb-4
          | > Carlos Quiroz
        h1.font-weight-thin.mb-4
          | - Full Stack Developer
</template>

<script>
export default {
  name: 'Index'
}
</script>

<style lang="scss" scoped>
.wrapper {
  width: 220px;
  display: flex;
  flex-wrap: wrap;
  h1 {
    font-size: 22px;
  }
}
</style>
