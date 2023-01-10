<script>
export default{
    data(){
        return{
            navList: [
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
                    text: "Collectibles",
                    url: "#",
                    current: false,
                },
                {
                    text: "Videos",
                    url: "#",
                    current: false,
                },
                {
                    text: "Fans",
                    url: "#",
                    current: false,
                },
                {
                    text: "News",
                    url: "#",
                    current: false,
                },
                {
                    text: "Shop",
                    url: "#",
                    current: false,
                },
            ]
        }
    }
}
</script>

<template>
    <div class="header-container">
        <nav>
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="Dc small logo">
            </div>
            <ul>
                <li v-for="navItem in navList" :class="(navItem.current) ? `active` : ``">
                    {{ navItem.text }}
                </li>
            </ul>
        </nav>
    </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

.header-container{
    width: 70%;
    margin: 0 auto;
}

// Utilizzare un nav "wrapper" all'interno del contenitore di header, per poter gestire meglio le dimensioni degli elementi
nav{
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 120px;
    .logo{
        padding: 1rem 0;
        height: 100%;
        // Necessario assegnare un'altezza al div contenitore dell'img poichè il nav container ha un'altezza fissa
        // Per far funzionare il padding, bisogna specificare anche l'altezza dell'img
        img{
            height: 100%;
        }
    }

    ul{
        display: flex;
        list-style-type: none;
        height: 100%;
    
        li{
            display: inline-block;
            padding: 0 0.8rem;
            text-transform: uppercase;
            line-height: calc(120px - 0.45rem);
            font-weight: 700;
            font-size: 0.9rem;
            border-bottom: 2px solid $WhiteColor;
    
            &.active{
                color: $MainColor;
                border-bottom: 2px solid $MainColor;
            }
    
            &:hover{
                color: $MainColor;
                border-bottom: 2px solid $MainColor;
                cursor: pointer;
            }
    }
    }

}

</style>
