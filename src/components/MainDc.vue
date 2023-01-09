<script>
export default{
    data(){
        return{
            iconList: [
                {
                    icon: "buy-comics-digital-comics.png",
                    text: "Digital Comics",
                    current: false,
                },
                {
                    icon: "buy-comics-merchandise.png",
                    text: "Merchandise",
                    current: false,
                },
                {
                    icon: "buy-comics-subscriptions.png",
                    text: "Subscription",
                    current: false,
                },
                {
                    icon: "buy-comics-shop-locator.png",
                    text: "Comic Shop Locator",
                    current: false,
                },
                {
                    icon: "buy-dc-power-visa.svg",
                    text: "Dc Power Visa",
                    current: false,
                }
            ]
        }
    }
}
</script>

<template>
    <section class="content-part">
        <div class="content-container">
            <h3>--> Content goes here </h3>
        </div>
        <img src="../assets/img/" alt="">
    </section>
    
    <section class="icons-nav">
        <ul>
            <li v-for="iconItem in iconList">                
                <img :src="`../assets/img/${iconItem.icon}`" alt="">
                {{ iconItem.text }}
            </li>
        </ul>
    </section>
</template>

<style lang="scss" scoped>
@use "../styles/general.scss" as *;
@use "../styles/partials/variables" as *;

.content-part{
    background-color: $BlackColor;
    padding: 3rem 0;
    .content-container{
        width: 70%;
        margin: 0 auto;
        color: $WhiteColor;
    }

};
.icons-nav{
    background-color: $MainColor;
    padding: 4rem 0;
    
    ul{
        width: 70%;
        margin: 0 auto;
        list-style-type: none;
        color: $WhiteColor;
        li{
            display: inline-block;
            padding: 0 1.5rem;
        }
    }

}
</style>
