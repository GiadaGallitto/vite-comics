<script>
export default{
    data(){
        return{
            toolList: [
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
            ]
        }
    }
}
</script>

<template>
    <section class="footer-container">
        <div class="nav-part">
            <div class="double-list">
                <ul>
                    <li><h4>Dc Comics</h4></li>
                    <li v-for="toolItem in toolList">
                        {{ toolItem.text }}
                    </li>
                </ul>
                <ul>
                    <li><h4>Shop</h4></li>
                    <li>Inserire frase originale</li>
                </ul>
            </div>

            <ul>
                <li>Ciao</li>
                <li>Inserire frase originale</li>
            </ul>

            <ul>
                <li>Ciao</li>
                <li>Inserire frase originale</li>
            </ul>
        </div>
        <div class="logo-part">

        </div>
    </section>
</template>

<style lang="scss" scoped>
@use "../styles/general.scss" as *;
@use "../styles/partials/variables" as *;

.footer-container{
    .nav-part{
        width: 70%;
        margin: 3rem auto;
        display: flex;
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
        color: $BlackColor;
    }
}

</style>
