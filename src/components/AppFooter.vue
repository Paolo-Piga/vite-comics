<script>
    export default{
        name: `AppFooter`,
        data() {
            return {
                VtComics: [
                    {
                        text: "Characters",
                        url: `#`,
                    },
                    {
                        text: "Comics",
                        url: `#`,
                    },
                    {
                        text: "Movies",
                        url: `#`,
                    },
                    {
                        text: "TV",
                        url: `#`,
                    },
                    {
                        text: "Games",
                        url: `#`,
                    },
                    {
                        text: "Collectibles",
                        url: `#`,
                    },
                    {
                        text: "Videos",
                        url: `#`,
                    },
                    {
                        text: "Fans",
                        url: `#`,
                    },
                    {
                        text: "News",
                        url: `#`,
                    },
                    {
                        text: "Shop",
                        url: `#`,
                    }
                ]
            }
        }
    }
</script>

<template>
    <div class="component-container">
        <div class="container">
            <div class="nav-menu">
                <div class="left">
                    <div class="dc-comics">
                        <div class="title">
                            VT COMICS
                        </div>
                        <ul >
                            <li v-for="(link,index) in dcComics" :key="index">
                                <a href="#">{{ link.text }}</a>
                            </li>
                        </ul>
                    </div>
                    <div class="shop">
                        <div class="title">
                            SHOP
                        </div>
                        <ul >
                            <li v-for="(link,index) in shop" :key="index">
                                <a href="#">{{ link.text }}</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="center">
                    <div class="dc">
                        <div class="title">
                            DC
                        </div>
                        <ul >
                            <li v-for="(link,index) in dc" :key="index">
                                <a href="#">{{ link.text }}</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="right">
                    <div class="sites">
                        <div class="title">
                            SITES
                        </div>
                        <ul >
                            <li v-for="(link,index) in sites" :key="index">
                                <a href="#">{{ link.text }}</a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
            <div class="dc-logo"></div>
        </div>
    </div>
</template>


<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;


.component-container {
    background-image: url(../assets/img/jumbotron.jpg);
    
}
.container {
    height: 50vh;
    display: flex;
    justify-content: space-between;
}
.nav-menu {
    display: flex;
    margin-top: 5%;
    gap: 2vw;
}
.dc-logo {
    background-image: url(../assets/img/dc-logo-bg.png);
    background-repeat: no-repeat;
    background-position: center;
    width: 50%;
}
.title {
    color: white;
    font-size: 18px;
    font-weight: bold;
    margin-bottom: 10%;
}
.dc-comics {
    margin-bottom: 15%;
}
li {
    list-style: none;

    a {
        text-decoration: none;
        color: #959595;
        font-size: 14px;
        line-height: 150%;
    }
    
}
</style>