<template>
  <main>
      <section class="h500">
          <div class="site-lg-container bg-light specs d-flex flex-column justify-content-center align-items-center text-center p-5">
              <div class="container d-flex flex-column justify-content-center align-items-center">
                    <h2 class="pointed">Our specialities</h2>
                    <span class="subtitle">
                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Sequi, praesentium?
                    </span>
                    <hr class="orange-rule">
                    <div class="row justify-content-center g-0 w-75">
                        <div class="col-3">
                            <div class="spec-card d-flex flex-column justify-content-center">
                                <img src="../assets/svg/svg-0.svg" alt="icon">
                                <h4>Knowing</h4>
                                <span class="subtitle">
                                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                                </span>
                            </div>
                        </div>
                        <div class="col-3">
                            <div class="spec-card d-flex flex-column justify-content-center">
                                <img src="@/assets/svg/svg-0.svg" alt="icon">
                                <h4>Knowing</h4>
                                <span class="subtitle">
                                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                                </span>
                            </div>
                        </div>
                        <div class="col-3">
                            <div class="spec-card d-flex flex-column justify-content-center">
                                <img src="@/assets/svg/svg-0.svg" alt="icon">
                                <h4>Knowing</h4>
                                <span class="subtitle">
                                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                                </span>
                            </div>
                        </div>
                        <div class="col-3">
                            <div class="spec-card d-flex flex-column justify-content-center">
                                <img src="@/assets/svg/svg-0.svg" alt="icon">
                                <h4>Knowing</h4>
                                <span class="subtitle">
                                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                                </span>
                            </div>
                        </div>
                    </div>
              </div>
          </div>
      </section>

      <section class="h500 member">
          <div class="container d-flex justify-content-center">
              <div class="row w-75 g-0 justify-content-center">
                  <div class="col-6">
                      <div class="member-image">
                          <img src="@/assets/img/h1-img-01.jpg" alt="founder">
                      </div>
                  </div>
                  <div class="col-6 d-flex align-items-center">
                      <div class="member-description bg-light p-5">
                          <h3>Jason BickFord</h3>
                          <span class="subtitle">Founder and Executive Director</span>
                          <hr class="orange-rule">
                          <p class="subtitle">
                              Lorem ipsum dolor sit, amet consectetur adipisicing elit. Labore voluptates, animi doloribus quam laboriosam dolorem quasi.
                          </p>
                          <div class="social-icons">
                              <i class="fab fa-linkedin-in"></i>
                              <i class="fab fa-facebook"></i>
                              <i class="fab fa-twitter"></i>

                          </div>
                      </div>

                  </div>
              </div>
          </div>
      </section>
  </main>
</template>

<script>
export default {
    name: 'Main',
}
</script>

<style lang="scss" scoped>
@import '@/styles/globals.scss';

main {
    background: $bg-grey;
}

// SPECS SECTION 
.specs {
    position: relative;
    top: -60px;
    h2 {
        font-size: 3rem;
    }
}

.spec-card {
    font-size: 12px;
    display: flex;
    justify-content: center;
    align-items: center;
    // padding: 30px;
    h4{
        font-size: 1rem;
    }
    img {
        max-width: 100%;
        object-fit: contain;
        margin-bottom: 1rem;
    }
    
}

// MEMBERS SECTION 

.member-image {
    img {
        width: 100%;
    }
}

.member-description {
    position: relative;
    left: -50px;
    font-size: 12px;
    .social-icons {
        color: $orange;
        i {
            margin-right: .5rem;
            font-size: 1rem;
            cursor: pointer;
            &:hover {
                color: black;
            }
        }
    }
}



</style>