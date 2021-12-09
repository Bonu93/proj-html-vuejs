<template>
  <div id="app">
    <Header :navList="headerMenu"/>

    <Main />

    <Footer />

  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import Main from '@/components/Main.vue'
import Footer from '@/components/Footer.vue'



export default {
  name: 'App',
  components: {
    Header, 
    Main, 
    Footer,
    
  }, 
  data() {
    return {
      headerMenu: [
        'Homes',
        'Pages',
        'Blog',
        'Shop',
        'Events', 
        'Elements',

      ],
    }
  },
}
</script>

<style lang="scss">
@import '@/styles/globals.scss';

</style>
