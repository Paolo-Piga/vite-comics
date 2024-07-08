<script>
import buyComicsDigitalComics from '../assets/img/buy-comics-digital-comics.png';
import buyComicsMerchandise from '../assets/img/buy-comics-merchandise.png';
import buyComicsShopLocator from '../assets/img/buy-comics-shop-locator.png';
import buyComicsSubscriptions from '../assets/img/buy-comics-subscriptions.png';
import buyDcPowerVisa from '../assets/img/buy-dc-power-visa.svg';




    export default {
        name :'AppPay',
        data() {
            return {
                images:[
                    {
                        image: buyComicsDigitalComics,
                        text: "DIGITAL COMICS"
                    },
                    {
                        image: buyComicsMerchandise,
                        text: "VT MERCHANDISE"
                    },
                    {
                        image: buyComicsSubscriptions,
                        text: "SUBSCRIPTION"
                    },
                    {
                        image: buyComicsShopLocator,
                        text: "COMIC SHOP LOCATOR"
                    },
                    {
                        image: buyDcPowerVisa,
                        text: "VT POWER VISA"
                    },
                    
                ],
            }
        }
    }
</script>

<template>
    <div class="component-container">
        <div class="container" >
            <div class="purchase" v-for="(purchase,index) in images" :key="index">
                <a href="#"><div class="icon"><img :src="purchase.image" alt=""></div> <div class="text">{{ purchase.text }}</div></a>
            </div>
        </div>
    </div>
</template>


<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

.component-container {
    background-color: $bluedc; 
}
.container {
    @include center(horizontal);
    height: 20vh;
    color: white;
    justify-content: space-between;
}
.purchase {
    a {
        @include center(horizontal);
        text-decoration: none;
        color: white;
        gap: 5px;
    }

    .icon {
        width: 50px;
        height: 50px;
        img {
        height: 100%;
        }
    }
}
</style>