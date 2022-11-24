<script>
    export default {
        name: 'AppSocial', 
        data(){
            return{
                socials: [
            {
                name: 'facebook',
                image: '../assets/footer-facebook.png'
            }, 
            {
                name: 'periscope',
                image: '../assets/footer-periscope.png'
            }, 
            {
                name: 'pinterest',
                image: '../assets/footer-pinterest.png'
            }, 
            {
                name: 'twitter',
                image: '../assets/footer-twitter.png'
            }, 
            {
                name: 'youtube',
                image: '../assets/footer-youtube.png'
            }
        ]
            }
        }
    }
</script>

<template>
    <div v-for="social in socials">
        <img :src="social.image" :alt="social.name">
    </div>
</template>

<style scoped>
    div{
        padding-left: .625rem;
    }
    img{
        width: 1.25rem;
        height: 1.25rem;
        border-radius: 50%;
    }
</style>