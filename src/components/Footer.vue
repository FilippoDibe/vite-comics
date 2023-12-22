<script>
export default {
    name: 'Footer',
}
</script>
<template>
    <div class="middle-blue-bar">
        <div class="content-container">
            <a href="#" class="blue-bar-item">
                <img src="/img/buy-comics-digital-comics.png" alt="Digital Comics" class="blue-bar-icon"> DIGITAL COMICS
            </a>
            <a href="#" class="blue-bar-item">
                <img src="/img/buy-comics-merchandise.png" alt="DC Merchandise" class="blue-bar-icon"> DC MERCHANDISE
            </a>
            <a href="#" class="blue-bar-item">
                <img src="/img/buy-comics-subscriptions.png" alt="Subscription" class="blue-bar-icon"> SUBSCRIPTION
            </a>
            <a href="#" class="blue-bar-item">
                <img src="/img/buy-comics-shop-locator.png" alt="Comic Shop Locator" class="blue-bar-icon"> COMIC SHOP
                LOCATOR
            </a>
            <a href="#" class="blue-bar-item">
                <img src="/img/buy-dc-power-visa.svg" alt="DC Power Visa" class="blue-bar-icon"> DC POWER VISA
            </a>
        </div>
    </div>

    <div class="footer-content">
        <div class="list-container">
            <div class="footer-section">
                <div class="dc-comics-column">
                    <h5>DC COMICS</h5>
                    <ul>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">TV</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Videos</a></li>
                        <li><a href="#">News</a></li>
                    </ul>
                </div>
                <div class="shop-colum">
                    <h5>SHOP</h5>
                    <ul>
                        <li><a href="#">Shop DC</a></li>
                        <li><a href="#">Shop DC Collectibles</a></li>
                    </ul>
                </div>
            </div>


            <div class="footer-section">
                <h5>DC</h5>
                <ul>
                    <li><a href="#">Terms Of Use</a></li>
                    <li><a href="#">Privacy policy (New)</a></li>
                    <li><a href="#">Ad Choices</a></li>
                    <li><a href="#">Advertising</a></li>
                    <li><a href="#">Jobs</a></li>
                    <li><a href="#">Subscriptions</a></li>
                    <li><a href="#">Talent Workshops</a></li>
                    <li><a href="#">CPSC Certificates</a></li>
                    <li><a href="#">Ratings</a></li>
                    <li><a href="#">Shop Help</a></li>
                    <li><a href="#">Contact Us</a></li>
                </ul>
            </div>

            <!-- Ripeti per le altre sezioni come "SITES", ecc. -->

            <div class="footer-section">
                <h5>SITES</h5>
                <ul>
                    <li><a href="#">DC</a></li>
                    <li><a href="#">MAD Magazine</a></li>
                    <li><a href="#">DC Kids</a></li>
                    <li><a href="#">DC Universe</a></li>
                    <li><a href="#">DC Power Visa</a></li>
                    <!-- Altri link se necessario -->
                </ul>
            </div>
        </div>
        <div class="footer-section-img">
            <img src="/img/dc-logo-bg.png" alt="">
        </div>
    </div>
    <div class="footer-last-row">
        <div class="footer-signup">
            <button>SIGN-UP NOW!</button>
        </div>
        <div class="footer-social">
            <span>FOLLOW US</span>
            <!-- Qui inserisci le icone social -->
            <a href="#"><img src="/img/footer-facebook.png" alt="Facebook"></a>
            <a href="#"><img src="/img/footer-twitter.png" alt="Twitter"></a>
            <a href="#"><img src="/img/footer-youtube.png" alt="YouTube"></a>
            <a href="#"><img src="/img/footer-pinterest.png" alt="Pinterest"></a>
            <a href="#"><img src="/img/footer-periscope.png" alt="Periscope"></a>

            <!-- Altri link social se necessario -->
        </div>
    </div>
</template>
  

<style lang="scss" scoped>
.middle-blue-bar {
    background-color: #007dc3;
    padding: 50px 0;
    width: 100vw;


    .content-container {
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 20px;


        .blue-bar-item {
            color: white;
            text-decoration: none;
            display: flex;
            align-items: center;
            gap: 10px;
            font-size: 20px;


            .blue-bar-icon {
                width: auto;
                height: 50px;
            }

            &:hover {
                text-decoration: underline;
            }
        }
    }
}

.footer-content {
    background-image: url('/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    width: 100vw;
    text-align: start;




    display: flex;
    justify-content: space-evenly;
}

.footer-section {
    color: white;
    margin: 0 20px;

    h5 {
        font-size: 20px;
    }

    ul {
        list-style-type: none;
        padding: 0;
    }

    a {
        color: grey;
        font-size: 13px;

        &:hover {
            color: white;
        }
    }


}

.list-container {
    display: flex;
    text-align: start;
    padding-top: 50px;
    padding-left: 100px;

}

.footer-last-row {
    display: flex;
    justify-content: space-around;
    align-items: center;
    padding: 30px 50px;
    background-color: #303030;

    .footer-signup {
        button {
            background-color: transparent;
            border: 1px solid #0056b3;
            color: white;
            padding: 10px 20px;
            font-size: 14px;
            cursor: pointer;
            transition: background-color 0.3s ease;

            &:hover {
                background-color: #0056b3;
            }
        }
    }

    .footer-social {
        display: flex;
        align-items: center;
        gap: 10px;

        span {
            color: #0056b3;
            font-size: 20px;
            margin-right: 20px;
        }

        a {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background-color: #555;
            transition: background-color 0.3s ease;

            &:hover {
                background-color: #0056b3;
            }

            img {
                width: 20px;
                height: auto;
            }
        }
    }
}
</style>