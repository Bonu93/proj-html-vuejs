<template>
  <main>
      <section class="h500">
          <div class="site-lg-container bg-light specs d-flex flex-column justify-content-center align-items-center text-center p-5">
              <div class="container">
                    <h2 class="pointed">Our specialities</h2>
                    <span class="subtitle">
                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Sequi, praesentium?
                    </span>
                    <hr class="orange-rule">
                    <div class="row">
                        <div class="col-3">
                            <div class="spec-card d-flex flex-column justify-content-center p-2 w-75">
                                <img src="../assets/svg/svg-0.svg" alt="icon">
                                <h4>Knowing</h4>
                                <span class="subtitle">
                                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                                </span>
                            </div>
                        </div>
                        <div class="col-3">
                            <div class="spec-card d-flex flex-column justify-content-center p-2 w-75">
                                <img src="@/assets/svg/svg-0.svg" alt="icon">
                                <h4>Knowing</h4>
                                <span class="subtitle">
                                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                                </span>
                            </div>
                        </div>
                        <div class="col-3">
                            <div class="spec-card d-flex flex-column justify-content-center p-2 w-75">
                                <img src="@/assets/svg/svg-0.svg" alt="icon">
                                <h4>Knowing</h4>
                                <span class="subtitle">
                                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                                </span>
                            </div>
                        </div>
                        <div class="col-3">
                            <div class="spec-card d-flex flex-column justify-content-center p-2 w-75">
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

      <section class="h700 member">
          <div class="container">
              <div class="row g-0">
                  <div class="col-6">
                      <div class="member-image">
                          <img src="@/assets/img/h1-img-01.jpg" alt="founder">
                      </div>
                  </div>
                  <div class="col-6">
                      <div class="member-description bg-light">
                          <h3>Jason BickFord</h3>
                          <span class="subtitle">Founder and Executive Director</span>
                          <hr class="orange-rule">
                          <p class="subtitle">
                              Lorem ipsum dolor sit, amet consectetur adipisicing elit. Labore voluptates, animi doloribus quam laboriosam dolorem quasi. Ut reprehenderit distinctio excepturi magnam deleniti ipsam nisi expedita. Autem amet tenetur ut! Quasi.
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
    h4{
        font-size: 1rem;
    }
    img {
        max-width: 60%;
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



</style>