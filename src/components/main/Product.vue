<template>
    <div class="product">
        <div class="product-wrap">
            <h1>PRODUCT</h1>
            <div data-aos="fade-right">
                <v-img src="@/assets/razer_monitor.png"></v-img>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Product',
};
</script>

<style lang="scss" scoped>
.product {
    height: 100vh;
    h1 {
        transition: all 0.2s;
    }
}
.product:hover h1 {
    color: #00ff00;
}
.product-wrap {
    width: 1000px;
    margin: 0 auto;
    h1 {
        text-align: center;
        color: white;
        margin: 100px;
    }
    div {
        width: 400px;
    }
}
</style>
