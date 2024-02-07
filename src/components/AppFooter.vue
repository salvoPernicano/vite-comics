<script>
export default {
    name: 'AppFooter'
}
</script>

<template>
    <footer>
        <div class="footerLinks">
            <div class="linksContainer">

                <div class="leftLinks">
                    <h3>Dc Comics</h3>
                    <ul>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">TV</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Videos</a></li>
                        <li><a href="#">News</a></li>
                    </ul>
                    <h3>Shop</h3>
                    <ul>
                        <li><a href="#">Shop Dc</a></li>
                        <li><a href="#">Shop Dc collectibles</a></li>
                    </ul>
                </div>
                <div class="rightLinks">
                    <div>
    
                        <h3>DC</h3>
                        <ul>
                            <li><a href="#">Terms of use</a></li>
                            <li><a href="#">Privacy policy</a></li>
                            <li><a href="#">Ad choises</a></li>
                            <li><a href="#">Advertising</a></li>
                            <li><a href="#">Jobs</a></li>
                            <li><a href="#">Subscriptions</a></li>
                            <li><a href="#">Talent workshops</a></li>
                            <li><a href="#">CPSC certificates</a></li>
                            <li><a href="#">Ratings</a></li>
                            <li><a href="#">Shop help</a></li>
                            <li><a href="#">Contact us</a></li>
                        </ul>
                    </div>
                    <div>
    
                        <h3>Sites</h3>
                        <ul>
                            <li><a href="#">DC</a></li>
                            <li><a href="#">MAD Magazine</a></li>
                            <li><a href="#">DC Kids</a></li>
                            <li><a href="#">DC UNiverse</a></li>
                            <li><a href="#">DC Power Visa</a></li>
                        </ul>
                    </div>
                </div>
            </div>
            <img  id="bigLogo" src="../assets/img/dc-logo-bg.png" alt="">
        </div>

        <div class="signUp">
            <button>Sign-up Now!</button>
            <div class="socialIcons">
                <h3>Follow us</h3>
                <ul>
                    <li><img src="../assets/img/footer-facebook.png" alt=""></li>
                    <li><img src="../assets/img/footer-twitter.png" alt=""></li>
                    <li><img src="../assets/img/footer-youtube.png" alt=""></li>
                    <li><img src="../assets/img/footer-pinterest.png" alt=""></li>
                    <li><img src="../assets/img/footer-periscope.png" alt=""></li>
                </ul>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

.footerLinks {
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    background-attachment: fixed;
    background-position: center;
    padding: 2em;
    display: flex;
    justify-content: space-around;
    gap: 20px;
    color: white;
    height: calc(50vh - 120px);
    position: relative;
    h3 {
        margin-bottom: 1em;

        &:nth-of-type(2) {
            margin-top: 1em;
        }
    }

    ul {
        list-style: none;
        line-height: 130%;
       

        a {
            color: grey;
            text-decoration: none;
        }
    }
};
#bigLogo{
    scale: 1.6;
}

.linksContainer{
    display: flex;
}
.rightLinks {
    display: flex;
    gap: 20px;
}

.signUp {
    background-color: $siteLighterBlack;
    display: flex;
    justify-content: space-around;
    align-items: center;
    padding: 2em;
    height: 120px;
    position: fixed;
    bottom: 0;
    left: 0;
    right: 0;

    button {
        background-color: transparent;
        border: 2px solid $siteBlue;
        color: white;
        text-transform: uppercase;
        padding: 10px 20px;
        font-size: 1rem;
    }

    .socialIcons {
        display: flex;
        align-items: center;

        h3 {
            color: $siteBlue;
            text-transform: uppercase;
            margin-right: 10px;
        }

        ul {
            display: flex;
            align-items: center;
            list-style: none;
            gap: 15px;
        }
    }
}</style>