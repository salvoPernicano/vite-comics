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
@use '../styles/partials/variables' as *;
.upperMain{
    background-color: $siteBlack;
    text-align: center;
    padding: 3.5em;
    height: 50%;
}
.lowerMain{
    background-color: $siteBlue;
    text-align: center;
    padding: 3em;
    height: 50%;
}
h1{
    color: white;
}
</style>