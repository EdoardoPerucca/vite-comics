<script>
export default {
    data() {
        return {

            linksShop: [
                {
                    image: 'img/buy-comics-digital-comics.png',
                    text: 'digital comics'
                },
                {
                    image: 'img/buy-comics-merchandise.png',
                    text: 'dc merchandise'
                },
                {
                    image: 'img/buy-comics-subscriptions.png',
                    text: 'subscription'
                },
                {
                    image: 'img/buy-comics-shop-locator.png',
                    text: 'comic shop locator'
                },
                {
                    image: 'img/buy-dc-power-visa.svg',
                    text: 'dc power visa'
                },
            ],
        }
    }
}
</script>

<template>
    <div id="nav-shop">
        <nav>
            <ul>
                <li v-for="linkShop in linksShop">
                    <img :src="linkShop.image" alt="">
                    {{ linkShop.text }}
                </li>
            </ul>
        </nav>

    </div>
</template>

<style scoped lang="scss">
#nav-shop {
    background-color: #0282f9;
    color: white;
    height: 100px;

    nav {
        display: flex;
        align-items: center;
        max-width: 1000px;
        margin: auto;
        height: 100%;
        width: 100%;
    }

    ul {
        display: flex;
        justify-content: space-around;
        width: 100%;
        gap: 20px;

        li {
            display: flex;
            align-items: center;
            gap: 10px;
            text-transform: uppercase;
            font-size: .8em;

            img {
                width: 30px;
            }
        }
    }
}
</style>