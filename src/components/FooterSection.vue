<script>
export default {
    data() {
        return {

        }
    }
}
</script>

<template>
    <div>
        <div id="footer-container">
            <div id="footer-inner">
                <div id="footer-left">

                    <button>Sign-Up Now</button>
                </div>

                <div id="footer-right">
                    <h3>follow us</h3>

                    <div id="footer-right-icon">
                        <i class="fa-brands fa-facebook-f icon"></i>
                        <i class="fa-brands fa-twitter icon"></i>
                        <i class="fa-brands fa-youtube icon"></i>
                        <i class="fa-brands fa-pinterest-p icon"></i>
                        <i class="fa-solid fa-location-dot icon"></i>

                    </div>

                </div>

            </div>
        </div>

    </div>
</template>

<style scoped lang="scss">
#footer-container {
    height: 80px;
    background-color: #303030;

    #footer-inner {
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 100%;
        max-width: 1000px;
        margin: auto;
        text-transform: uppercase;

        button {
            padding: 1em;
            text-transform: uppercase;
            border: 2px solid #0282f9;
            background-color: #303030;
            color: white;
        }

        #footer-right {
            display: flex;
            align-items: center;
            gap: 1em;

            h3 {
                color: #057ff7;
            }

            #footer-right-icon {
                display: flex;
                gap: 1em;


                .icon {
                    background-color: #797979;
                    color: #303030;
                    padding: .5em;
                    border-radius: 50%;
                }
            }
        }
    }
}
</style>