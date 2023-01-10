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
    </section>
    
    <section class="icons-nav">
        <div class="icons-container">
            <div class="banner-element" v-for="iconItem in iconList">
                <img :src="`/img/${iconItem.icon}`" alt="icon">
                <p>
                    {{ iconItem.text }}
                </p>          
            </div>
        </div>
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
    
    .icons-container{
        width: 75%;
        margin: 0 auto;
        color: $WhiteColor;
        display: flex;
        justify-content: space-between;
        .banner-element{
            display: flex;
            align-items: center;
            margin: 0 0.5rem;

            img{
                width: 55px;
            }

            p{
                margin-left: 1rem;
            }
        }
    }
}
</style>
