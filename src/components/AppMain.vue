<script>

export default {
    name : 'AppMain',
}
</script>

<template>
    <main>
        <div class="upperMain">
            <h1>--Content goes here--</h1>
        </div>
        <div class="lowerMain">
            <h1>Lorem, ipsum dolor.</h1>
        </div>
    </main>
</template>

<style lang="scss" scoped>
@import '../styles/partials/variables';
.upperMain{
    background-color: $siteBlack;
    text-align: center;
    padding: 3em;
}
.lowerMain{
    background-color: $siteBlue;
    text-align: center;
    padding: 3em;
}
h1{
    color: white;
}
</style>