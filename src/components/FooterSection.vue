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
                        <img src="img/footer-facebook.png" alt="">
                        <img src="img/footer-twitter.png" alt="">
                        <img src="img/footer-youtube.png" alt="">
                        <img src="img/footer-pinterest.png" alt="">
                        <img src="img/footer-periscope.png" alt="">
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


            }
        }
    }
}
</style>