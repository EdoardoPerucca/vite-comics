<script>
export default {
    data() {
        return {

            links: [
                'characters',
                'comics',
                'movies',
                'tv',
                'games',
                'collectibles',
                'videos',
                'fans',
                'news',
                'shop'
            ],

            activeIndex: [],
        }

    },

    methods: {
        newActiveIndex(newIndex) {
            this.activeIndex = newIndex
        }
    }
}
</script>

<template>
    <div id="header-container">
        <div id="header-inner">
            <div id="logo">
                <img src="img/favicon.ico" alt="">
            </div>

            <nav>
                <ul>
                    <li>
                        <a href="#" v-for="(link, index) in links" :class="index == activeIndex ? 'active' : ''"
                            @click="newActiveIndex(index)">
                            {{ link }}
                        </a>
                    </li>
                </ul>
            </nav>

        </div>

    </div>
</template>

<style scoped lang="scss">
#header-container {
    background-color: white;
    height: 100px;
    width: 100%;

    #header-inner {
        display: flex;
        flex-flow: row nowrap;
        justify-content: space-between;
        align-items: center;
        height: 100%;
        max-width: 1000px;
        margin: auto;

        #logo img {
            width: 4em;
        }

        nav {
            height: 100%;


            ul {
                display: flex;
                flex-flow: row nowrap;
                height: 100%;


                li {
                    display: flex;
                    align-items: center;
                    text-transform: uppercase;
                    font-size: .8em;
                    gap: 15px;


                    a {
                        display: flex;
                        align-items: center;
                        text-decoration: none;
                        color: #615856;
                        height: 100%;

                        &.active {
                            color: #0282f9;
                            border-bottom: 3px solid #0282f9;


                        }

                    }

                }

            }
        }

    }
}
</style>