<template>
    <div class="col-6">
        <div class="feature"
        v-for="(feature, i) in data.roleData"
        :key="`feature-${i}`"
        >
            <div class="bar-info d-flex justify-content-between">
                <h4>{{feature.feature}}</h4>
                <h4>{{feature.percentage}}</h4>
            </div>
            <div class="bar">
                <div class="loaded-bar" :style="{width:`${feature.percentage}`}"></div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Features',
    props: {
        data: Object,
    }
};
</script>

<style lang="scss" scoped>
@import "@/styles/globals.scss";

.bar {
    background: grey;
    height: 1px;
    margin-bottom: 1rem;
    .loaded-bar {
        background: $orange;
        height: 3px;
        // width: 78%;
        position: relative;
        top: -2px;
    }
}

.bar-info {
    h4 {
        font-size: 1.2rem;
    }
}
</style>
