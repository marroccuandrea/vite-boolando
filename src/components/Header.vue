<script>
export default {

}
</script>

<template>
    <header>
        <div class="banner">
            <div>
                <ul>
                    <li><a href="#">Donna</a></li>
                    <li><a href="#">Uomo</a></li>
                    <li><a href="#">Bambino</a></li>
                </ul>
            </div>
            <img class="logo" src="../assets/scss/img/boolean-logo.png" alt="">
            <div>
                <ul>
                    <li><i class="fa-regular fa-user"></i></li>
                    <li><i class="fa-regular fa-heart"></i></li>
                    <li><i class="fa-solid fa-bag-shopping"></i></li>
                </ul>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

header {
    display: flex;
    align-items: center;
    height: 70px;
    background-color: $orange-h;
    color: $bianco;

}

.banner {
    max-width: 1200px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin: 0 auto;
}

ul {
    display: flex;
    list-style: none;

    li {
        padding: 15px;

        a {
            text-decoration: none;
            color: $bianco;
        }
    }
}
</style>
