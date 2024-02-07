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
          <ul>
            <li>
                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                <span>Dc merchandie</span>
            </li>
            <li>
                <img src="../assets/img/buy-comics-merchandise.png" alt="">
                <span>Dc merchandie</span>
            </li>
            <li>
                <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                <span>Dc merchandie</span>
            </li>
            <li>
                <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                <span>Dc merchandie</span>
            </li>
            <li>
                <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                <span>Dc merchandie</span>
            </li>
          </ul>
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
    display: flex;
    justify-content: center;
    height: 50%;
  ul{
    display: flex;
    align-items: center;
    gap: 50px;
    color: white;
    text-transform: uppercase;
    list-style: none;
    li{
        display: flex;
        align-items: center;
        img{
            width: 50px;
            height: 50px;
            object-fit: contain;
        }
    }
  }
}
h1{
    color: white;
}
</style>