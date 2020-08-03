<template lang="pug">
  v-app
    v-navigation-drawer(v-model="drawer", :mini-variant="miniVariant", :clipped="clipped", fixed, app)
      v-list
        v-list-item(v-for='(item, i) in items' :key='i' :to='item.to' router exact)
          v-list-item-action
            v-icon {{ item.icon }}
          v-list-item-content
            v-list-item-title(v-text='item.title')

    v-app-bar(:clipped-left='clipped' fixed app)
      v-app-bar-nav-icon(@click.stop='drawer = !drawer')
      v-btn(icon='' @click.stop='miniVariant = !miniVariant')
        v-icon mdi-{{ `chevron-${miniVariant ? 'right' : 'left' }` }}
      v-toolbar-title(v-text='title')
      v-spacer
      social-media
    v-main
      v-container
        nuxt
    v-footer.d-flex.justify-end(absolute app)
      span 💻 with love 💙
</template>

<script>
import SocialMedia from '@/components/utils/SocialMedia'

export default {
  components: {
    SocialMedia
  },

  data () {
    return {
      clipped: true,
      drawer: false,
      items: [
        {
          icon: 'mdi-home-assistant',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-information-outline',
          title: 'About',
          to: '/about'
        },
        {
          icon: 'mdi-account-box',
          title: 'Contact',
          to: '/contact'
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Carlos Quiroz 🚀'
    }
  }
}
</script>
<style lang="scss" scoped></style>
