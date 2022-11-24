<script>
    export default {
        name: 'AppCard', 
        data(){
            return {
                images: [
                {
                    src: '../assets/buy-comics-digital-comics.png',
                    imgName: 'DIGITAL COMICS'
                },
                {
                    src: '../assets/buy-comics-merchandise.png',
                    imgName: 'DC MERCHANDISE' 
                },
                {
                    src: '../assets/buy-comics-subscriptions.png',
                    imgName: 'SUBSCRIPTION' 
                },
                {
                    src: '../assets/buy-comics-shop-locator.png',
                    imgName: 'COMIC SHOP LOCATOR' 
                },
                {
                    src: '../assets/buy-dc-power-visa',
                    imgName: 'DC POWER VISA' 
                }
            ]
        }
    }
}
</script>

<template>
    <div v-for="image in images" class="flex align-items-center">
        <img :src="image.src" :alt="imgName">
        <span>{{image.imgName}}</span>
    </div>
</template>

<style scoped>
    div{
        padding: 3.125rem 0;
    }
    img{
        width: 1.875rem;
    }
</style>