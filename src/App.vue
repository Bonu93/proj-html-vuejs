<template>
  <div id="app">
    <Header :navList="headerMenu"/>

    <Main 
    :data="mainData"
    />

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

      mainData: {
        specsData: [
          {
            title: 'Knowing',
            img: 'svg-0.svg',
            text: 'Lorem ipsum dolor sit amet, quis consect'
          },
          {
            title: 'Selling',
            img: 'svg-1.svg',
            text: 'Lorem ipsum dolor sit amet, quis consect'
          },
          {
            title: 'Learning',
            img: 'svg-2.svg',
            text: 'Lorem ipsum dolor sit amet, quis consect'
          },
          {
            title: 'Contact',
            img: 'svg-3.svg',
            text: 'Lorem ipsum dolor sit amet, quis consect'
          }

        ],

        calendarData: [
          {
            day: '07',
            date: 'Jan, 2022',
            name: 'Melbourne Coaching',
            time: '9:00 am - 5:00pm, Jan 7,2022',
            location: 'Cambridge, MA 02138, USA'
          },
          {
            day: '11',
            date: 'Jan, 2022',
            name: 'New York Coaching',
            time: '9:00 am - 5:00pm, Jan 11,2022',
            location: 'Cambridge, MA 02138, USA'
          },
          {
            day: '21',
            date: 'Jan, 2022',
            name: 'London Coaching',
            time: '9:00 am - 5:00pm, Jan 21,2022',
            location: 'Cambridge, MA 02138, USA'
          },
        ],

        roleData: [
           {
             feature: 'Mentorship',
             percentage: '78%'
           },
           {
             feature: 'Education',
             percentage: '95%'
           },
           {
             feature: 'Learning',
             percentage: '65%'
           },
           {
             feature: 'Motivation',
             percentage: '83%'
           }
        ],


      },

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
