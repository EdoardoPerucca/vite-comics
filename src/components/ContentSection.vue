<script>
export default {
    data() {
        return {

        }
    }
}
</script>

<template>
    <div id="content">
        <div id="content-inner">
            <h2>Content goes here</h2>
        </div>

    </div>
</template>

<style scoped lang="scss">
#content {
    background-color: black;
    color: white;
    height: 80px;

    #content-inner {
        display: flex;
        align-items: center;
        max-width: 1000px;
        height: 100%;
        margin: auto;
    }

}
</style>