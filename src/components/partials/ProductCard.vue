<script>
export default {
    props: {
        vestito: Object,
    }
}
</script>

<template>
    <div class="card">
        <div class="card-images">
            <img :src="`/img/${vestito.frontImage}`" alt="1">
            <img class="secondary-image" :src="`/img/${vestito.backImage}`" alt="1">
            <div class="favourite">
                <i class="fa-solid fa-heart"></i>
            </div>
            <div class="badges">
                <span v-for="discount in  vestito.badges " :key=discount :class="discount.type"
                    class="badge discount">{{ discount.value }}</span>
                <!-- <span class="badge tag">sostenibilità</span> -->
            </div>
        </div>

        <div class="card-text">
            <div class="brand">{{ vestito.brand }}</div>
            <div class="product-name">{{ vestito.name }}</div>
            <div class="price">
                <span>{{ vestito.price }}&#8364</span>
                <!-- <del>{{ vestito.price }}</del> -->
            </div>
        </div>
    </div>

</template>


<style lang="scss" scoped>
img {
    width: 100%;

}

.card {
    width: calc(100% / 3);
    padding: 0 10px;
    margin-bottom: 20px;


    .card-images {
        position: relative;
        cursor: pointer;

        &:hover .secondary-image {
            display: block;
        }

        .favourite:hover {
            color: red;
        }



        .favourite {
            position: absolute;
            background-color: white;
            top: 20px;
            right: 0;
            padding: 21px 14px;
        }

        .secondary-image {
            display: none;
            position: absolute;
            top: 0;
            left: 0;
        }
    }

    .card-text .price {
        font-size: .9rem;

        span {
            padding-right: 5px;
            color: red;
            font-weight: 700;
        }
    }

    .card-text .product-name {
        font-weight: 700;
        text-transform: uppercase;
    }


}

.card .card-images .badges .badge {
    padding: 5px 10px;
    color: white;
    font-weight: 700;
    text-transform: capitalize;
}

.card .card-images .badges .badge.discount {
    background-color: red;
}

.card .card-images .badges .badge.tag {
    background-color: green;
}

.card .card-images .badges {
    position: absolute;
    bottom: 15px;
    left: 0;
}
</style>