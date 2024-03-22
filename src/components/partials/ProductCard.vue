<script>
export default {

}
</script>

<template>
    <div class="card">
        <div class="card-images">
            <img src="../../data/1.webp" alt="1">
            <img class="secondary-image" src="../../data/1b.webp" alt="1">
            <div class="favourite">
                <i class="fa-solid fa-heart"></i>
            </div>
            <div class="badges">
                <span class="badge discount">-50%</span>
                <span class="badge tag">sostenibilità</span>
            </div>
        </div>

        <div class="card-text">
            <div class="brand">Levi's</div>
            <div class="product-name">RELAXED fit tee UNISEX</div>
            <div class="price">
                <span>14,99 &euro;</span>
                <del>29,99 &euro;</del>
            </div>
        </div>
    </div>
    <div class="card">
        <div class="card-images">
            <img src="../../data/2.webp" alt="2">
            <img class="secondary-image" src="../../data/2b.webp" alt="2">
            <div class="favourite">
                <i class="fa-solid fa-heart"></i>
            </div>
            <div class="badges">
                <span class="badge discount">-50%</span>
                <span class="badge tag">sostenibilità</span>
            </div>
        </div>

        <div class="card-text">
            <div class="brand">Levi's</div>
            <div class="product-name">RELAXED fit tee UNISEX</div>
            <div class="price">
                <span>14,99 &euro;</span>
                <del>29,99 &euro;</del>
            </div>
        </div>
    </div>
    <div class="card">
        <div class="card-images">
            <img src="../../data/3.webp" alt="3">
            <img class="secondary-image" src="../../data/3b.webp" alt="3">
            <div class="favourite">
                <i class="fa-solid fa-heart"></i>
            </div>
            <div class="badges">
                <span class="badge discount">-50%</span>
                <span class="badge tag">sostenibilità</span>
            </div>
        </div>

        <div class="card-text">
            <div class="brand">Levi's</div>
            <div class="product-name">RELAXED fit tee UNISEX</div>
            <div class="price">
                <span>14,99 &euro;</span>
                <del>29,99 &euro;</del>
            </div>
        </div>
    </div>
    <div class="card">
        <div class="card-images">
            <img src="../../data/4.webp" alt="4">
            <img class="secondary-image" src="../../data/4b.webp" alt="4">
            <div class="favourite">
                <i class="fa-solid fa-heart"></i>
            </div>
            <div class="badges">
                <span class="badge discount">-50%</span>
                <span class="badge tag">sostenibilità</span>
            </div>
        </div>

        <div class="card-text">
            <div class="brand">Levi's</div>
            <div class="product-name">RELAXED fit tee UNISEX</div>
            <div class="price">
                <span>14,99 &euro;</span>
                <del>29,99 &euro;</del>
            </div>
        </div>
    </div>
    <div class="card">
        <div class="card-images">
            <img src="../../data/5.webp" alt="5">
            <img class="secondary-image" src="../../data/5b.webp" alt="5">
            <div class="favourite">
                <i class="fa-solid fa-heart"></i>
            </div>
            <div class="badges">
                <span class="badge discount">-50%</span>
                <span class="badge tag">sostenibilità</span>
            </div>
        </div>

        <div class="card-text">
            <div class="brand">Levi's</div>
            <div class="product-name">RELAXED fit tee UNISEX</div>
            <div class="price">
                <span>14,99 &euro;</span>
                <del>29,99 &euro;</del>
            </div>
        </div>
    </div>
    <div class="card">
        <div class="card-images">
            <img src="../../data/6.webp" alt="6">
            <img class="secondary-image" src="../../data/6b.webp" alt="6">
            <div class="favourite">
                <i class="fa-solid fa-heart"></i>
            </div>
            <div class="badges">
                <span class="badge discount">-50%</span>
                <span class="badge tag">sostenibilità</span>
            </div>
        </div>

        <div class="card-text">
            <div class="brand">Levi's</div>
            <div class="product-name">RELAXED fit tee UNISEX</div>
            <div class="price">
                <span>14,99 &euro;</span>
                <del>29,99 &euro;</del>
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