<template>
    <div class="visual">
        <v-carousel cycle height="100vh" hide-delimiter-background show-arrows-on-hover>
            <v-carousel-item v-for="(item, i) in items" :src="item.src" :key="i"></v-carousel-item>
        </v-carousel>
    </div>
</template>

<script>
export default {
    name: 'Name',
    data() {
        return {
            items: [
                {
                    src:
                        'https://assets2.razerzone.com/images/pnx.assets/4e1df9019f354d30707d2b44f673a0cb/a-1920x700-desktop-razerbook13.jpg',
                },
                {
                    src:
                        'https://assets2.razerzone.com/images/pnx.assets/4e1df9019f354d30707d2b44f673a0cb/kaira-pro-homepage-large.jpg',
                },
                {
                    src:
                        'https://assets2.razerzone.com/images/pnx.assets/4e1df9019f354d30707d2b44f673a0cb/wireless-flagship-a-1920x700-desktop.jpg',
                },
            ],
        };
    },
};
</script>

<style lang="scss" scoped>
.visual {
}
</style>
