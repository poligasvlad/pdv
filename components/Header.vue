<template>
    <header class="header">
        <div class="container">
            <div class="header-wrapper">
              <div class="logo"><img src="~/assets/images/logo.svg" alt="logotype"></div>
              <deskNav v-if="flag"></deskNav>
              <mobNav v-else></mobNav>

            </div>
        </div>
    </header>
</template>
<script>

export default {
  name: 'Header',
  components: {
    mobNav: () => import('~/components/mobileNav.vue'),
    deskNav: () => import('~/components/deskNav.vue')
  },
  data() {
    return {
      flag: true,
    }
  },
  mounted () {
    this.checkSize();
    window.addEventListener('resize', this.checkSize)
  },
  methods: {
    checkSize(){
      this.flag = innerWidth >= 980
    }
  }
}
</script>

<style lang="scss">
@import '~/assets/styles/component/header.scss';
</style>
