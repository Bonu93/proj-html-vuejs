<template>
  <header class="d-flex flex-column">
      <div class="top-header site-lg-container py-3 d-flex justify-content-between align-items-center">
          <h1 class="pointed">Everlead</h1>

          <ul class="d-flex align-items-center">
              <li v-for="(item, i) in navList" :key="`nav-item-${i}`">
                    
                    <a href="#"
                    class="menu-item"
                    >
                        {{ item }}
                    </a>
              </li>

              <li>
                  <a href="">
                    <i class="fas fa-search"></i>
                  </a>
              </li>
              <li>
                  <a href="">
                   <i class="fas fa-list-ul"></i>
                  </a>
              </li>
              
          </ul>
      </div>

      <div class="flex-grow-1 d-flex align-items-center">
          <div class="slider site-lg-container d-flex">
              <button class="slider-btn left-arrow">&#10229;</button>
              <div class="slider-content flex-grow-1">
                  <div class="container">
                      <div class="row">
                          <div class="col-6">

                            <h2 class="pointed">Our Team</h2>
                            <p>
                                Lorem ipsum dolor sit amet consectetur adipisicing elit. Harum rem dolor obcaecati deserunt quam ut beatae recusandae ratione enim iure perspiciatis quod eligendi dicta quae eum ullam cupiditate, aspernatur exercitationem.
                            </p>
                            <div class="cta d-flex">
                                <div class="site-btn site-btn-prim">
                                    <div class="btn-txt">
                                        Read More
                                    </div>
                                    <div class="btn-arrow">
                                        &#10230;
                                    </div>
                                </div>


                                <div class="site-btn site-btn-orange mx-3">
                                    <div class="btn-txt">
                                        Purchase
                                    </div>
                                    <div class="btn-arrow">
                                        &#10230;
                                    </div>
                                </div>
                                

                                

                            </div>

                          </div>
                      </div>
                  </div>
              </div>
              <button class="slider-btn right-arrow">&#10230;</button>
          </div>

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
    height: 700px;
    background-image: url('../assets/img/rev-slider-main-home-img-03.jpg');
    background-size: cover;
    background-position-y: 50%;
    background-position-x: center;
    h1 {
        font-size: 1.5rem;
    }
    ul {
        list-style: none;
        height: 30px;
        font-size: 12px;
        li {
            display: flex;
            align-items: center;
            margin: 0 .5rem;
            a {
                text-decoration: none;
                color: black;
                text-transform: uppercase;
                &:hover {
                    color: $orange;
                    &::before {
                        color: $orange;
                    }
                }
            }
        }
    }
}

.menu-item::before {
    content: '\27F6';
    color: transparent;
    font-size: 1rem;
}

.slider-content {
    margin-left: 100px;
    h2 {
        font-size: 5rem;
    }
}


</style>