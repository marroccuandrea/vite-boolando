<script>
import ProductCard from './partials/ProductCard.vue';
export default {
    components: {
        ProductCard
    }
}
</script>

<template>
    <main>
        <div class="container">
            <ProductCard />

        </div>
    </main>
</template>

<style lang="scss" scoped>
main {
    padding: 30px 0;

    .container {
        display: flex;
        flex-wrap: wrap;
        max-width: 1200px;
        margin: 0 auto;


    }
}
</style>
