<script>
import { headerMenues } from '../data/menues'

export default {
    computed: {
        mainMenu() {
            return headerMenues.main
        },
        socialMenu() {
            return headerMenues.social
        }
    }
}
</script>

<template>
    <header>
        <div class="banner">
            <div>
                <ul>
                    <li v-for="(item, index) in mainMenu" :key="`m-${index}`"><a :href="item.href">{{ item.text }}</a>
                    </li>

                </ul>
            </div>
            <img class="logo" src="../assets/scss/img/boolean-logo.png" alt="">
            <div>
                <ul>
                    <li v-for="(item, index) in socialMenu" :key="`s-${index}`"><a :href="item.href"
                            v-html="`${item.text}`"></a>
                    </li>

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
    justify-content: center;
    height: 70px;
    background-color: $orange-h;
    color: $bianco;

}

.banner {
    width: 1200px;
    display: flex;
    justify-content: space-between;
    align-items: center;
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
