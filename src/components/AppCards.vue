<script>
export default {
    name: "AppCards",
    data() {
        return {

        }
    },

    props: {
        img: String,
        title: String,
    }
}
</script>

<template>
    <div id="single-card">
        <div id="img-card"><img :src="img" alt=""></div>
        <div id="text-card"> {{ title }}</div>
    </div>
</template>

<style scoped lang="scss">
#single-card {
    width: 150px;
    height: 250px;
    background-color: #1c1c1c;
    text-align: start;

    #img-card {
        width: 150px;
        height: 200px;
        overflow-y: hidden;

        img {
            width: 100%;
        }
    }

    #text-card {
        text-transform: uppercase;
        font-size: .7em;
        padding-top: .5em;
    }

}
</style>