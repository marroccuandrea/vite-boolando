<script>
import { footerMenues } from '../data/menues'
export default {
    computed: {
        socialMenu() {
            return footerMenues.social
        }
    }
}
</script>

<template>
    <footer>
        <div class="foot-btm">
            <div class="footer-sx">
                <h4>Boolando s.r.l.</h4>
                <nav>
                    <ul>
                        <!-- Da fare dinamica -->
                        <li><a href=""></a>Informazioni legali</li>
                        <li><a href=""></a>Informativa sulla privacy</li>
                        <li><a href=""></a>Diritto di recesso</li>
                    </ul>
                </nav>
            </div>
            <div class="footer-dx">
                <h5>Trovaci anche su</h5>
                <nav>
                    <ul>
                        <li v-for="(item, index) in socialMenu" :key="`s-${index}`"><a :href="item.href"
                                v-html="`${item.text}`"></a></li>

                    </ul>
                </nav>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

footer {
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: black;
    height: 90px;
    color: $bianco;
}

.foot-btm {
    width: 1200px;
    display: flex;
    justify-content: space-between;
    align-items: center;

}

h4 {
    font-size: 1rem;
    padding-bottom: 10px;
}

h5 {
    padding-bottom: 10px;
    font-size: 0.9rem;
}

ul {
    display: flex;
    list-style: none;

    li {
        padding-right: 10px;
        font-size: 0.8rem;

        a {
            color: $bianco;
        }

        i {
            font-size: 1rem;

        }
    }
}
</style>