<template>
    <main>
        <!-- SPECIALITIES SECTION -->
        <Specs :data="data"/>
        
        <!-- MEMBERS SECTION -->
        <section class="h500 member d-flex justify-content-center">
            <div class="container d-flex justify-content-center">
                <div class="row w-75 g-0 justify-content-center">
                    <div class="col-6">
                        <div class="member-image">
                            <img
                                src="@/assets/img/h1-img-01.jpg"
                                alt="founder"
                            />
                            <div class="arrows">
                                <a href="#">&#10229;</a>
                                <a href="#">&#10230;</a>
                            </div>
                        </div>
                    </div>
                    <div class="col-6 d-flex align-items-center">
                        <div class="member-description p-5">
                            <h3>Jason BickFord</h3>
                            <span class="subtitle"
                                >Founder and Executive Director</span
                            >
                            <hr class="orange-rule" />
                            <p class="subtitle">
                                Lorem ipsum dolor sit, amet consectetur
                                adipisicing elit. Labore voluptates, animi
                                doloribus quam laboriosam dolorem quasi.
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
            <div class="overlay-image">
                <img src="../assets/svg/svg-4.svg" alt="">
            </div>
        </section>
        <!-- COACHING-CALENDAR SECTION -->
        <section
            class="h700 coaching d-flex justify-content-center align-items-center"
        >
            <div class="container d-flex justify-content-center">
                <div class="row w-75">
                    <div class="col-5">
                       <Calendar :data="data"/>
                    </div>
                </div>
            </div>
        </section>
        <!-- ROLE SECTION -->
        <section
            class="h500 role d-flex justify-content-center align-items-center"
        >
            <div
                class="container d-flex justify-content-center align-items-center"
            >
                <div class="row w-75">
                    <div class="col-6">
                        <h3 class="pointed">Creative Leader</h3>
                        <hr class="orange-rule" />
                        <p class="subtitle">
                            Lorem ipsum, dolor sit amet consectetur adipisicing
                            elit. Sint, laudantium quaerat nisi fugit ad quae
                            temporibus sunt alias itaque illo velit vitae sed
                            natus, libero, explicabo necessitatibus ipsa ducimus
                            iure!
                        </p>
                        <a href="#" class="read-more">READ MORE</a>
                    </div>

                    
                    <Features :data="data"/>
                    
                </div>
            </div>
        </section>
        <!-- NEWS SECTION -->
        <section
            class="news h700 d-flex flex-column justify-content-center align-items-center"
        >
            <h2 class="pointed">Latest News</h2>
            <span class="subtitle"
                >Lorem ipsum dolor sit amet consectetur adipisicing elit.</span
            >
            <hr class="orange-rule" />
            <div class="slider site-lg-container d-flex">
                <button class="slider-btn left-arrow">&#10229;</button>
                <div
                    class="container d-flex justify-content-center align-items-center"
                >
                    <div class="row w-75">
                        <div class="col-4">
                            <div class="news-card">
                                <div class="news-image">
                                    <img
                                        src="../assets/img/h1-blog-img-02.jpg"
                                        alt="blog-thumb"
                                    />
                                    <div class="news-label">
                                        <i class="fas fa-tag"></i> Business,
                                        Leading
                                    </div>
                                </div>
                                <div class="news-info">
                                    <span class="subtitle date"
                                        ><i class="far fa-clock"></i>May 5,
                                        2019</span
                                    >
                                    <span class="subtitle author"
                                        ><i class="far fa-user"></i>Amanda
                                        Doe</span
                                    >
                                </div>
                                <h3>Next investment</h3>
                                <p class="preview subtitle">
                                    Lorem ipsum dolor sit amet consectetur
                                    adipisicing elit. Iste dicta dolores ipsum
                                    tempora corporis, quod, consequatur, sequi
                                    odit tempore officiis alias blanditiis
                                    corrupti molestiae temporibus expedita
                                    accusamus quas quidem molestias.
                                </p>
                                <a href="#" class="read-more">Read More</a>
                            </div>
                        </div>
                        <div class="col-4">
                            <div class="news-card">
                                <div class="news-image">
                                    <img
                                        src="../assets/img/h1-blog-img-04.jpg"
                                        alt="blog-thumb"
                                    />
                                    <div class="news-label">
                                        <i class="fas fa-tag"></i> Business,
                                        Leading
                                    </div>
                                </div>
                                <div class="news-info">
                                    <span class="subtitle date"
                                        ><i class="far fa-clock"></i>May 5,
                                        2019</span
                                    >
                                    <span class="subtitle author"
                                        ><i class="far fa-user"></i>Amanda
                                        Doe</span
                                    >
                                </div>
                                <h3>Team building</h3>
                                <p class="preview subtitle">
                                    Lorem ipsum dolor sit amet consectetur
                                    adipisicing elit. Iste dicta dolores ipsum
                                    tempora corporis, quod, consequatur, sequi
                                    odit tempore officiis alias blanditiis
                                    corrupti molestiae temporibus expedita
                                    accusamus quas quidem molestias.
                                </p>
                                <a href="#" class="read-more">Read More</a>
                            </div>
                        </div>
                        <div class="col-4">
                            <div class="news-card">
                                <div class="news-image">
                                    <img
                                        src="../assets/img/h1-blog-img-01.jpg"
                                        alt="blog-thumb"
                                    />
                                    <div class="news-label">
                                        <i class="fas fa-tag"></i> Business,
                                        Leading
                                    </div>
                                </div>
                                <div class="news-info">
                                    <span class="subtitle date"
                                        ><i class="far fa-clock"></i>May 5,
                                        2019</span
                                    >
                                    <span class="subtitle author"
                                        ><i class="far fa-user"></i>Amanda
                                        Doe</span
                                    >
                                </div>
                                <h3>New Business Day</h3>
                                <p class="preview subtitle">
                                    Lorem ipsum dolor sit amet consectetur
                                    adipisicing elit. Iste dicta dolores ipsum
                                    tempora corporis, quod, consequatur, sequi
                                    odit tempore officiis alias blanditiis
                                    corrupti molestiae temporibus expedita
                                    accusamus quas quidem molestias.
                                </p>
                                <a href="#" class="read-more">Read More</a>
                            </div>
                        </div>
                    </div>
                </div>
                <button class="slider-btn right-arrow">&#10230;</button>
            </div>
            <div class="overlay-image">
                <img src="../assets/svg/svg-4.svg" alt="">
            </div>
        </section>
        <!-- TESTIMONIALS SECTION -->
        <section
            class="testimonials h400 d-flex flex-column align-items-center"
        >
            <div
                class="site-lg-container d-flex flex-column align-items-center"
            >
                <h2 class="bg-title">Testimonials.</h2>
            </div>
            <div class="slider site-lg-container d-flex">
                <button class="slider-btn left-arrow">&#10229;</button>
                <div class="slider-content flex-grow-1">
                    <div class="container d-flex justify-content-center">
                        <div class="row w-75 d-flex justify-content-center">
                            <div
                                class="col-8 text-center d-flex justify-content-center"
                            >
                                <div
                                    class="testimonial d-flex flex-column align-items-center"
                                >
                                    <div class="testimonial-img">
                                        <img
                                            src="@/assets/img/h3-img-04.png"
                                            alt="testimonial"
                                        />
                                    </div>
                                    <h3 class="testimonial-name">
                                        Cynthia Clark
                                    </h3>
                                    <p class="testimonial-motto subtitle">
                                        "Lorem ipsum dolor, sit amet consectetur
                                        adipisicing elit. Fuga numquam
                                        dignissimos dolores autem magnam."
                                    </p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <button class="slider-btn right-arrow">&#10230;</button>
            </div>
        </section>
        <!-- VIDEO SECTION  -->
        <section
            class="video h700 d-flex justify-content-center align-items-center"
        >
            <div class="player">
                <i class="fas fa-play"></i>
            </div>
            <div class="buttons">
                <div
                    class="circle d-flex justify-content-center align-items-center"
                >
                    <svg
                        xmlns="http://www.w3.org/2000/svg"
                        viewBox="0 0 87 87"
                        style="height: 40px"
                        fill="#ffffff"
                    >
                        <path
                            d="M55.4 81.5c6.1-11.1 5.2-16.1-4.3-24.3 6.1-3.5 9.5-8.5 9.1-15.7-.5-8.2-7.7-14.7-16.3-14.6-8.5.1-15.6 6.7-15.9 15-.3 8.5 5.9 15.8 14.3 16.6 1.4.1 2.8.2 4.2.5 5.9 1.2 10.2 6.7 9.8 12.6-.4 6.4-5.5 11.4-11.8 11.7-19.6.9-38.6-14.8-41.3-34C-.1 26.9 14.4 6.8 36.4 2.8c22.3-4 43.4 10 48.1 32 4.3 20-8.6 41.2-28.4 46.7h-.7z"
                        />
                    </svg>
                </div>
                <div
                    class="cart d-flex justify-content-center align-items-center"
                >
                    <svg
                        xmlns="http://www.w3.org/2000/svg"
                        viewBox="0 0 24 24"
                        style="height: 16px"
                        fill="#ee2852"
                    >
                        <circle cx="9" cy="21" r="2" />
                        <circle cx="20" cy="21" r="2" />
                        <path
                            d="M23.8 5.4c-.2-.3-.5-.4-.8-.4H6.8L6 .8C5.9.3 5.5 0 5 0H1C.4 0 0 .4 0 1s.4 1 1 1h3.2L5 6.2v.1l1.7 8.3C7 16 8.2 17 9.6 17H19.4c1.5 0 2.7-1 3-2.4L24 6.2c0-.3 0-.6-.2-.8z"
                        />
                    </svg>
                </div>
            </div>
        </section>
        <!-- MAP SECTION -->
        <section
            class="map h500 d-flex justify-content-center align-items-center"
        >
            <div class="container d-flex justify-content-center">
                <div class="row w-75">
                    <div class="col-6 d-flex justify-content-center align-items-center">
                        <div class="map">
                            <img
                                src="../assets/img/h1-contact-rev-01.png"
                                alt="map"
                            />
                            <div class="pointer-1">
                                <img src="../assets/img/h1-contact-rev-02.png" alt="">
                                <div class="pointer-label">
                                    <h4>New York Coaching</h4>
                                    <a href="" class="read-more">Read More</a>
                                </div>
                            </div>
                            <div class="pointer-2">
                                <img src="../assets/img/h1-contact-rev-02.png" alt="">
                                <div class="pointer-label">
                                    <h4>Oslo Coaching</h4>
                                    <a href="" class="read-more">Read More</a>
                                </div>
                            </div>
                            <div class="pointer-3">
                                <img src="../assets/img/h1-contact-rev-02.png" alt="">
                                <div class="pointer-label">
                                    <h4>Adelaide Coaching</h4>
                                    <a href="" class="read-more">Read More</a>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col-6">
                        <h2 class="pointed">Contact us</h2>
                        <span class="subtitle">
                            Lorem, ipsum dolor sit amet consectetur adipisicing
                            elit.
                        </span>
                        <hr class="orange-rule" />
                        <form action="message" class="message">
                            <div class="d-flex">
                                <input
                                    type="text"
                                    id="name"
                                    placeholder="Your Name"
                                />
                                <input
                                    type="email"
                                    id="email"
                                    placeholder="Your Email"
                                />

                            </div>
                            <textarea
                                name=""
                                id=""
                                rows="2"
                                placeholder="Write your message"
                            ></textarea>
                            <div class="site-btn site-btn-orange">
                                <div class="btn-txt">Send</div>
                                <div class="btn-arrow">&#10230;</div>
                            </div>
                        </form>
                    </div>
                </div>
            </div>
        </section>
        <!-- CLIENTS SECTION -->
        <section class="clients d-flex justify-content-center align-items-center">
            <div class="container d-flex justify-content-center">
                <div class="row w-75 g-0">
                    <div class="col-12 d-flex justify-content-between">

                        <div class="client-img">
                            <img src="../assets/img/h4-clients-img-03.png" alt="">
                            <img src="../assets/img/h4-clients-img-04-1.png" alt="">
                        </div>
                        <div class="client-img">
                            <img src="../assets/img/h4-clients-img-05.png" alt="">
                            <img src="../assets/img/h4-clients-img-06-1.png" alt="">
                        </div>
                        <div class="client-img">
                            <img src="../assets/img/h4-clients-img-07.png" alt="">
                            <img src="../assets/img/h4-clients-img-08-1.png" alt="">
                        </div>
                        <div class="client-img">
                            <img src="../assets/img/h4-clients-img-09.png" alt="">
                            <img src="../assets/img/h4-clients-img-10-1.png" alt="">
                        </div>
                        <div class="client-img">
                            <img src="../assets/img/h4-clients-img-01.png" alt="">
                            <img src="../assets/img/h4-clients-img-02.png" alt="">
                        </div>
                    </div>
                </div>
            </div>
        </section>
        <!-- SCROLLUP BUTTON  -->
        <div class="scroll-up">
            <a href="#">&#8593;</a>
        </div>
    </main>
</template>

<script>
import Specs from '@/components/Specs.vue';
import Calendar from '@/components/Calendar.vue';
import Features from '@/components/Features.vue';


export default {
    name: "Main",
    props: {
        data: Object,
    },
    components: {
        Specs,
        Calendar,
        Features,
    }
};
</script>

<style lang="scss" scoped>
@import "@/styles/globals.scss";

main {
    background: $bg-main;
}


// MEMBERS SECTION
.member {
    position: relative;
    .overlay-image {
        position: absolute;
        top: -75px;
        left: 1000px;
        img {
            width: 400px;
        }
    }
}

.member-image {
    position: relative;
    .arrows {
        position: absolute;
        bottom: 0;
        background: $orange;
        padding: 0.8rem;
        a {
            color: white;
            text-decoration: none;
            margin: 0.5rem;
        }
    }
    img {
        width: 100%;
    }
}

.member-description {
    position: relative;
    z-index: 1;
    left: -50px;
    top: -15%;
    font-size: 12px;
    background: $white;
    .social-icons {
        color: $orange;
        i {
            margin-right: 0.5rem;
            font-size: 1rem;
            cursor: pointer;
            &:hover {
                color: black;
            }
        }
    }
}

// COACHING SECTION

.calendar {
    background-color: $white-alt;
}
.coaching {
    margin-right: 1rem;
    background-image: url("../assets/img/h1-img-09.jpg");
    background-position-y: 30%;
    background-size: cover;
    font-size: 12px;
    .calendar-title {
        box-shadow: rgba(33, 35, 38, 0.1) 0px 10px 10px -10px;
        background: $white-alt;
    }
    h4 {
        font-size: 1.2rem;
    }
    .date {
        background: $orange;
        color: white;
        height: 60px;
        width: 60px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        font-size: 10px;
        .day {
            display: block;
            font-size: 1rem;
        }
    }
}

// ROLE SECTION
.role {
    background: $white;
}


// NEWS SECTION
.news {
    position: relative;
    .overlay-image {
        position: absolute;
        top: -90px;
        left: 150px;
        img {
            width: 400px;
        }
    }
    h2 {
        font-size: 3rem;
    }
    .preview {
        overflow: hidden;
        text-overflow: ellipsis;
        display: -webkit-box;
        -webkit-line-clamp: 2;
        -webkit-box-orient: vertical;
    }
    .news-card {
        position: relative;
        z-index: 1;
        .news-info {
            font-size: 12px;
            .date {
                margin-right: 5px;
            }
            i {
                color: $orange;
                margin-right: 5px;
            }
        }

        .news-image {
            position: relative;
            margin-bottom: 1.5rem;
            .news-label {
                display: flex;
                justify-content: center;
                align-items: center;
                font-size: 10px;
                font-weight: 100;
                background: $orange;
                color: $white-alt;
                padding: 0.5rem;
                position: absolute;
                top: 90%;
                left: 55%;
                i {
                    margin-right: 5px;
                }
            }
            img {
                width: 100%;
            }
        }
    }
}

// TESTIMONIAL SECTION
.testimonials {
    position: relative;
    color: $white;
    background: #1e1c1c;
    overflow: hidden;
    .bg-title {
        color: $text-black-alt;
        text-align: center;
        font-size: 15rem;
        position: relative;
        top: -45px;
    }
    .slider {
        position: absolute;
        top: 110px;
    }
    .slider-btn {
        color: $white;
    }
    .testimonial-name {
        font-size: 1rem;
        margin-bottom: 1rem;
    }
    .testimonial-img {
        border-radius: 50%;
        border: 4px solid white;
        width: 100px;
        margin-bottom: 1rem;
        img {
            width: 100%;
        }
    }
}

//VIDEO SECTION
.video {
    margin-right: 1rem;
    position: relative;
    background-image: url("../assets/img/h1-img-04.jpg");
    background-size: cover;
    .player {
        color: $white;
        font-size: 3rem;
    }
    .buttons {
        position: absolute;
        right: -1rem;
        top: -1rem;
        .circle {
            background: $fucsia;
            margin-bottom: 10px;
            svg {
                width: 60%;
            }
        }
        .cart {
            padding: 12px 4px;
            background: $white;
            svg {
                width: 60%;
                fill: $fucsia;
            }
        }
    }
}

//MAP SECTION

.map {
    position: relative;
    .pointer-1 {
        position: absolute;
        top: 90px;
        left: 103px;
    }
    .pointer-2 {
        position: absolute;
        top: 48px;
        left: 234px;
    }
    .pointer-3 {
        position: absolute;
        top: 178px;
        left: 379px;
    }
    img {
        width: 100%;
    }
    .pointer-1,
    .pointer-2,
    .pointer-3 {
        cursor: pointer;
        img {
            width: 20px;
        }
        &:hover {
            .pointer-label {
                opacity: 1;
            }
        }
    }
}

.pointer-label {
    position: relative;
    top: 10px;
    left: -30px;
    padding: 1rem;
    background: $white-alt;
    box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
    opacity: 0;
    transition: opacity .5s ease;
    h4 {
        margin-bottom: 0;
    }

}

//FORM

.message {
    input,
    textarea {
        background: transparent;
        border: 0;
        border-bottom: 1px solid grey;
        outline: none;
    }
    input {
        width: 50%;
        // margin: 1rem;
    }
    textarea {
        width: 100%;
        margin-bottom: 2rem;
    }
    #email {
        margin-left: 1rem;
    }
}

// CLIENTS SECTION
.clients {
    padding: 5rem 0;
}
.client-img {
    cursor: pointer;
    
    img {
        width: 100%;
        &:last-child {
            display: none;
        }
    }
    &:hover {
        & img:first-child {
            display: none;
        }
        & img:last-child {
            display: inline-block;
        }
    }
}

.scroll-up {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 40px;
    height: 40px;
    background: $white;
    position: fixed;
    bottom: 100px;
    right: 20px;
    border-radius: 50%;
    box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
    a {
        text-decoration: none;
        color: $orange;
        display: block;
        height: 100%;
        font-size: 1.5rem;
    }
}
</style>


