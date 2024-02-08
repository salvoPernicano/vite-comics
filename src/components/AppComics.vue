<script>
export default {
    name : "AppComics",
  props: {
    propThumb : String,
    propSeries : String
  }
    }

</script>


<template>
    
        <div class="item">
                    <figure>
                        <img :src="propThumb" alt="item">
                    </figure>
                    <div class="comicType">
                        <span>{{ propSeries }}</span>

                    </div>
                </div>
</template>


<style lang="scss">
 .item{
        color: white;
        flex-basis: calc(100% / 6 - 10px);
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    figure{
    width: 80%;
    height: 300px;
        img{
            height: 100%;
            width: 100%;
            object-fit: cover;
        }
    }
    .comicType{
        padding: 10px;
        height: 50px;
    }
}</style>