<script>
export default {

}
</script>

<template>
    <footer>
        <div class="foot-btm">
            <div class="footer-sx">
                <h4>Boolando s.r.l.</h4>
                <nav>
                    <ul>
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
                        <li><i class="fa-brands fa-square-x-twitter"></i></li>
                        <li><i class="fa-brands fa-square-facebook"></i></li>
                        <li><i class="fa-brands fa-instagram"></i></li>
                        <li><i class="fa-brands fa-pinterest"></i></li>
                        <li><i class="fa-brands fa-youtube"></i></li>
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

        i {
            font-size: 1rem;
        }
    }
}
</style>