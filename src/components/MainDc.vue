<script>

</script>

<template>
    <section class="content-part">
        <div class="content-container">
            <h3>--> Content goes here </h3>
        </div>
    </section>
    
    <section class="icons-nav">
        <ul>
            <li>                
                Qui ci penso dopo... Trust the Process
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
    }

}
</style>
