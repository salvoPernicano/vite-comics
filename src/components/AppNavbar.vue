<script>

export default {
    name: 'AppNavbar',
    data(){
        return {
            ArrayLinksMenu : [
            {
                nome : 'Characters',
                link : '#',
                current : false
            },
            {
                nome : 'Comics',
                link : '#',
                current : true
            },
            {
                nome : 'Movies',
                link : '#',
                current : false
            },
            {
                nome : 'Tv',
                link : '#',
                current : false
            },
            {
                nome : 'Games',
                link : '#',
                current : false
            },
            {
                nome : 'Collectibles',
                link : '#',
                current : false
            },
            {
                nome : 'Videos',
                link : '#',
                current : false
            },
            {
                nome : 'Fans',
                link : '#',
                current : false
            },
            {
                nome : 'News',
                link : '#',
                current : false
            },
            {
                nome : 'Shop',
                link : '#',
                current : false
            }
            ]
        }
    }
}
</script>

<template>
    <header>
        <nav>
            <figure>
                <img src="../assets/img/dc-logo.png" alt="">
            </figure>
            <ul>
      <li v-for="(element,index) in ArrayLinksMenu" :key="index"><a href="#">{{element.nome}}</a></li>

            </ul>
        </nav>

    </header>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
 header{
    background-color: white;
    nav{
        display: flex;
        justify-content: space-around;
        align-items: center;
        ul{
            display: flex;
            align-items: center;
            list-style: none;
            gap: 10px;
            font-weight: bold;
            text-transform: uppercase;
            font-size: 0.9rem;
            a{
                text-decoration: none;
                color: $siteBlack;
                &:hover{
                    color: $siteBlue
                }
            }
        }
    };
    figure{
        display: flex;
        align-items: center;
        justify-content: center;
        img{
            padding: 1.5em;
            height: 120px
        }
    }
 };
 li{
    position: relative;
    height: 100%;
 }
 li::after {
    content: '';
    width: 0px;
    height: 5px;
    background-color: $siteBlue;
    position: absolute;
    top: 400%;
    left: 0;
    transition: all 0.3s
 };
 li:hover:after{
    width: 100%;
}
</style>