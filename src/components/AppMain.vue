<script>
import AppComics from '../components/AppComics.vue';
export default {
    name: 'AppMain',
    components :{
        AppComics
    },
    data() {
        return {
            comicsArray: [
  {
      "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
      "price": "$19.99",
      "series": "Action Comics",
      "type": "comic book",
  },
  {
      "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
      "price": "$3.99",
      "series": "American Vampire 1976",
      "type": "comic book",
  },
  {
      "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
      "price": "$16.99",
      "series": "Aquaman",
      "type": "graphic novel",
  },
  {
      "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
      "price": "$2.99",
      "series": "Batgirl",
      "type": "comic book",
  },
  {
      "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
      "price": "$3.99",
      "series": "Batman",
      "type": "comic book",
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
      "price": "$2.99",
      "series": "Batman Beyond",
      "type": "comic book",
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
      "price": "$3.99",
      "series": "Batman/Superman",
      "type": "comic book",
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
      "price": "$4.99",
      "series": "Batman/Superman Annual",
      "type": "comic book",
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
      "price": "$5.99",
      "series": "Batman: The Joker War Zone",
      "type": "comic book",
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
      "price": "$6.99",
      "series": "Batman: Three Jokers",
      "type": "comic book",
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
      "price": "$4.99",
      "series": "Batman: White Knight Presents: Harley Quinn",
      "type": "comic book",
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
      "price": "$16.99",
      "series": "Catwoman",
      "type": "graphic novel",
  },
]
        }
    }
}
</script>

<template>
    <main>
        <div class="upperMain">
            <div class="upperBg"></div>
            <div class="comicsContainer">
                <AppComics v-for="(element,index) in comicsArray"
                :propThumb="element.thumb"
                :propSeries="element.series"></AppComics>
                <!-- <AppComics/> -->
                <!-- <AppComics  v-for="(element,index) in comicsArray" 
                :key="index"
                :propsSrc="element.thumb"
                :propsSeries="element.series"/> -->
            </div>
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

.upperMain {
    background-color: $siteBlack;
    text-align: center;
}

.comicsContainer{
    padding: 3em;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    gap: 10px;
   
}
.upperBg {
    background-image: url(../assets/img/jumbotron.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    background-position: top;
    height: 50vh;
}

.lowerMain {
    background-color: $siteBlue;
    text-align: center;
    display: flex;
    justify-content: center;
    padding: 2em;

    ul {
        display: flex;
        align-items: center;
        gap: 50px;
        color: white;
        text-transform: uppercase;
        list-style: none;

        li {
            display: flex;
            align-items: center;

            img {
                width: 50px;
                height: 50px;
                object-fit: contain;
            }
        }
    }
}

h1 {
    color: white;
}</style>