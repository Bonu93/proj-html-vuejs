<template>
    <section class="h500">
            <div
                class="site-lg-container specs d-flex flex-column justify-content-center align-items-center text-center p-5"
            >
                <div
                    class="container d-flex flex-column justify-content-center align-items-center"
                >
                    <h2 class="pointed">Our specialities</h2>
                    <span class="subtitle">
                        Lorem ipsum dolor sit amet consectetur adipisicing elit.
                        Sequi, praesentium?
                    </span>
                    <hr class="orange-rule" />
                    <div class="row justify-content-center g-0 w-75">
                        <div class="col-3"
                        :key="`spec-${i}`"
                        v-for="(item, i) in data.specsData"
                        >
                            <div
                                class="spec-card d-flex flex-column justify-content-center"
                            >
                                <img :src="require(`@/assets/svg/${item.img}`)" :alt="item.title" />
                                <h4>{{ item.title }}</h4>
                                <span class="subtitle">
                                    {{item.text}}
                                </span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
</template>

<script>
export default {
    name: 'Specs',
    props: {
        data: Object,
    }

}
</script>

<style lang="scss" scoped>

@import "@/styles/globals.scss";

    .specs {
    position: relative;
    top: -60px;
    background: $white;
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
    h4 {
        font-size: 1rem;
    }
    img {
        max-width: 100%;
        object-fit: contain;
        margin-bottom: 1rem;
    }
}
</style>