<script>
import ProductCard from './partials/ProductCard.vue';
import { products } from '../data/db.json';
export default {
    data() {
        return {
            products
        }
    },
    components: {
        ProductCard
    }
}
</script>

<template>
    <main>
        <div class="container">
            <ProductCard v-for="product in this.products" :key="product.id" :vestito="product" />

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
