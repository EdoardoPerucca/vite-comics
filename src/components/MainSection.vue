<script>
export default {
    data() {
        return {

            mainColumns: [
                {
                    title: 'dc comics',
                    links: [
                        'characters',
                        'comics',
                        'movies',
                        'tv',
                        'games',
                        'videos',
                        'news'
                    ]
                },
                {
                    title: 'dc',
                    links: [
                        'terms of use',
                        'privacy policy (new)',
                        'ad choices',
                        'advertising',
                        'jobs',
                        'subscriptions',
                        'talent workshops',
                        'CPSC certificates',
                        'ratings',
                        'shop help',
                        'contact us'
                    ]
                },
                {
                    title: 'sites',
                    links: [
                        'DC',
                        'MAD magazine',
                        'DC kids',
                        'DC universe',
                        'DC power visa'
                    ]
                },
                {
                    title: 'shop',
                    links: [
                        'shop DC',
                        'shop DC collectibles'
                    ]
                },
            ]
        }
    }
}
</script>

<template>
    <div id="main">

        <nav>
            <div id="main-column" v-for="mainColumn in mainColumns">
                <strong> {{ mainColumn.title }} </strong>
                <ul>
                    <li v-for="link in mainColumn.links"> {{ link }}</li>
                </ul>
            </div>
        </nav>

        <div>
            <img id="img-logo" src="/img/dc-logo-bg.png" alt="">
        </div>

    </div>
</template>

<style scoped lang="scss">
#main {
    height: calc(100% - 360px);
    color: white;
    position: relative;
    overflow-y: hidden;
    max-width: 1000px;
    width: 100%;
    margin: auto;
    padding-top: 20px;

    nav {
        display: flex;
        flex-wrap: wrap;
        width: calc(100% / 3);
        width: 300px;
        gap: 20px;
        font-size: .7em;


        #main-column {

            strong {
                text-transform: uppercase;
                font-size: .9em;
            }

            li {
                color: #616a67;
            }

        }

    }


    #img-logo {
        width: 400px;
        position: absolute;
        top: -70px;
        right: 0px;
    }

}
</style>