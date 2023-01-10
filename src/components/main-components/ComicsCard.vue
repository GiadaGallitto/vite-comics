<script>
export default{
    data(){
        return{

        }
    },

    props: {
        imagePath: String,
        title: String
    }
}
</script>

<template>
    <div class="comics-card">
        <div class="image-box">
            <img :src="imagePath" />
        </div>
        <h4>{{ title }}</h4>
    </div>
</template>

<style lang="scss" scoped>
    .comics-card{
        width: calc((100% / 6) - 2rem);
        display: flex;
        flex-direction: column;
        margin: 0 1rem;
        .image-box{
            width: 100%;
            height: 60%;
            overflow: hidden;

            img{
                width: 100%;
            }
        }
    }
</style>