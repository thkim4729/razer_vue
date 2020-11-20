<template>
    <div class="main">
        <visual></visual>
        <product></product>

        <div id="top">
            <v-btn fab small color="white" @click="scrollToTop()">
                <v-icon>mdi-chevron-up</v-icon>
            </v-btn>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Main',
    components: {
        Visual: () => import('@/components/main/Visual.vue'),
        Product: () => import('@/components/main/Product.vue'),
    },
    methods: {
        scrollToTop() {
            window.scrollTo(0, 0);
        },
    },
};
</script>

<style lang="scss" scoped>
#top {
    position: fixed;
    bottom: 30px;
    right: 30px;
    z-index: 100000;
}
</style>
