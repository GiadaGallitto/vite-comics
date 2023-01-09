<script>
export default{
    data(){
        return{
            DcComicsList: [
                {
                    text: "Characters",
                    url: "#",
                    current: false,
                },
                {
                    text: "Comics",
                    url: "#",
                    current: true,
                },
                {
                    text: "Movies",
                    url: "#",
                    current: false,
                },
                {
                    text: "Tv",
                    url: "#",
                    current: false,
                },
                {
                    text: "Games",
                    url: "#",
                    current: false,
                },
                {
                    text: "Videos",
                    url: "#",
                    current: false,
                },
                {
                    text: "News",
                    url: "#",
                    current: false,
                },
            ],

            ShopList: [
                {
                    text: "Shop DC",
                    url: "#",
                    current: false,
                },
                {
                    text: "Shop DC Collectibles",
                    url: "#",
                    current: true,
                },
            ],

            DcList: [
                {
                    text: "Terms Of Use",
                    url: "#",
                    current: false,
                },
                {
                    text: "Privacy policy (New)",
                    url: "#",
                    current: true,
                },
                {
                    text: "Ad Choices",
                    url: "#",
                    current: false,
                },
                {
                    text: "Advertising",
                    url: "#",
                    current: false,
                },
                {
                    text: "Jobs",
                    url: "#",
                    current: false,
                },
                {
                    text: "Subscriptions",
                    url: "#",
                    current: false,
                },
                {
                    text: "Talent Workshops",
                    url: "#",
                    current: false,
                },
                {
                    text: "CPSC Certificates",
                    url: "#",
                    current: false,
                },
                {
                    text: "Ratings",
                    url: "#",
                    current: false,
                },
                {
                    text: "Shop Help",
                    url: "#",
                    current: false,
                },
                {
                    text: "Contact Us",
                    url: "#",
                    current: false,
                },
            ],

            SitesList: [
                {
                    text: "DC",
                    url: "#",
                    current: false,
                },
                {
                    text: "MAD Magazine",
                    url: "#",
                    current: false,
                },
                {
                    text: "DC Kids",
                    url: "#",
                    current: false,
                },
                {
                    text: "DC Universe",
                    url: "#",
                    current: false,
                },
                {
                    text: "DC Power Visa",
                    url: "#",
                    current: false,
                },
            ],
        }
    }
}
</script>

<template>
    <section class="footer-container">
        <div class="content-container">
            <div class="nav-part">
                <div class="double-list">
                    <ul>
                        <li><h4>Dc Comics</h4></li>
                        <li v-for="DcComicsItem in DcComicsList">
                            {{ DcComicsItem.text }}
                        </li>
                    </ul>
                    <ul>
                        <li><h4>Shop</h4></li>
                        <li v-for="ShopItem in ShopList">
                            {{ ShopItem.text }}
                        </li>
                    </ul>
                </div>
    
                <ul>
                    <li><h4>Dc</h4></li>
                    <li v-for="DcItem in DcList">
                        {{ DcItem.text }}
                    </li>
                </ul>
    
                <ul>
                    <li><h4>Sites</h4></li>
                    <li v-for="SitesItem in SitesList">
                        {{ SitesItem.text }}
                    </li>
                </ul>
            </div>
    
            <div class="logo-part">
                <img src="../assets/img/dc-logo-bg.png" alt="Big logo Dc">
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use "../styles/general.scss" as *;
@use "../styles/partials/variables" as *;

.footer-container{
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
    .content-container{
        width: 70%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        overflow: hidden;
        .nav-part{
            display: flex;
            padding: 3rem 0;
        }
        .logo-part{
            position: relative;

            img{
                position: absolute;
                top: -20%;
                right: 0;
            }
        }
    }

    ul{
        list-style-type: none;
        margin-right: 2rem;
        margin-bottom: 1rem;

        li{
            font-size: 0.9rem;
            line-height: 1.4rem;
            color: $SecondaryColor;
        }
    }

    h4{
        text-transform: uppercase;
        margin-bottom: 0.8rem;
        font-size: 1rem;
        color: $WhiteColor;
    }
}

</style>
