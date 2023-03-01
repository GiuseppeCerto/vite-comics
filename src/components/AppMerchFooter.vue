<template>
    <section class="merch_section">
        <div class="container menu_item_flex">
            <div class="merch_item">
                <img src="/images/buy-comics-digital-comics.png" alt="">
                <span>DIGITAL COMICS</span>
            </div>
            <div class="merch_item">
                <img src="/images/buy-comics-merchandise.png" alt="">
                <span>DC MERCHANDISE</span>
            </div>
            <div class="merch_item">
                <img src="/images/buy-comics-subscriptions.png" alt="">
                <span>SUBSCRIPTION</span>
            </div>
            <div class="merch_item">
                <img src="/images/buy-comics-shop-locator.png" alt="">
                <span>COMIC SHOP LOCATOR</span>
            </div>
            <div class="merch_item">
                <img src="/images/buy-dc-power-visa.svg" alt="">
                <span>DC POWER VISA</span>
            </div>
        </div>
    </section>

</template>
    
<script>
    export default {
        
    }
</script>
    
<style lang="scss" scoped>

    .container{
        width: 1100px;
    }

    .merch_section{
        background-color: rgba(2,130,249,255);
        padding: 45px 0;
        color: white;
        font-size: 15px;
    }

    .menu_item_flex{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .merch_item{
        display: flex;
        align-items: center;
        gap: 15px;
    }

    .merch_item img{
        width: 50px;
        height: 60px;
    }
</style>