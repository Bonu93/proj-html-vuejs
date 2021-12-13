<template>
  <div id="app">
    <Header :navList="headerMenu"/>

    <Main />

    <Footer
    :data="footerData"
     />

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

      footerData: {

        footerAbout: {
          listItem: 'We created Everlead to effectively become the stepping stone towards meeting all your goals & achieving business success',
        },

        footerTwitter: [
          {
            tweet: '@aliasadam Hi, can you please submit a ticket at https//t.co/lorem and one of our support agent'
          },
          {
            tweet: '@HenrySefa Check out our theme Gioia which has all the necessary elements to build a multivendor marketplace https//t.co/lorem'
          },
        ],

        footerLinks: [
          {
            text: 'About me',
            url: '/'
          },
          {
            text: 'About us',
            url: '/'
          },
          {
            text: 'Language packs',
            url: '/'
          },
          {
            text: 'Become a coach',
            url: '/'
          },
          {
            text: 'Monthly events',
            url: '/'
          },
        ],

        footerContacts: [
          {
            text: '457 BigBlue Street, NY 10013',
            icon: 'fas fa-map-marker-alt'
          },
          {
            text: '(315) 5512-2579',
            icon: 'fas fa-phone-alt',
          },
          {
            text: 'everlead@mikado.com',
            icon: 'far fa-envelope'
          }
        ],

      }
    }
  },
}
</script>

<style lang="scss">
@import '@/styles/globals.scss';

</style>
