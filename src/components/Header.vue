<template>
  <header>
      <div class="top-header site-lg-container py-3 d-flex justify-content-between align-items-center">
          <h1 class="pointed">Everlead</h1>

          <ul class="d-flex align-items-center">
              <li v-for="(item, i) in navList" :key="`nav-item-${i}`"
              class="mx-2"
              >
                    
                    <a href="#">
                    <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32"><path d="M4 15a1 1 0 001 1h19.586l-4.292 4.292a1 1 0 001.414 1.414l6-6a.99.99 0 00.292-.702V15c0-.13-.026-.26-.078-.382a.99.99 0 00-.216-.324l-6-6a1 1 0 00-1.414 1.414L24.586 14H5a1 1 0 00-1 1z"/></svg>
                        {{ item }}
                    </a>
              </li>
          </ul>
      </div>

      <div class="slider">

      </div>
  </header>
</template>

<script>
export default {
    name: 'Header',
    props: {
        navList: Array,
    },
}
</script>

<style lang="scss" scoped>
@import '@/styles/globals.scss';

header {
    height: 100vh;
    background-image: url('../assets/img/rev-slider-main-home-img-03.jpg');
    background-size: cover;
    background-position-y: 50%;
    background-position-x: center;
    ul {
        list-style: none;
        height: 30px;
        li {
            display: flex;
            align-items: center;
            a {
                text-decoration: none;
                color: black;
                text-transform: uppercase;
                svg {
                    fill: transparent;
                }
                &:hover {
                    color: $orange;
                    svg {
                        fill: $orange;
                    }
                }
            }
        }
    }
}

</style>