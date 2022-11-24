<script>
    import AppCard from './AppCard.vue';
    import AppFooterLink from './AppFooterLink.vue';
    import AppSocial from './AppSocial.vue';
    export default {
        name: 'AppFooter', 
        components: {
            AppCard, 
            AppFooterLink, 
            AppSocial
        }
    }
</script>

<template>
    <div id="footer-top">
        <div class="container flex space-between">
            <AppCard/>
        </div>
    </div>
    <div id="footer-center">
        <div class="container">
            <AppFooterLink/>
            <img src="../assets/dc-logo-bg.png" alt="">
        </div>
    </div>
    <div id="footer-bottom">
        <div class="container flex space-between">
            <button>SIGN UP NOW!</button>
            <div class="flex">
                <span>FOLLOW US</span>
                <!-- LINKIMAGE COMPONENT -->
                <AppSocial/>
            </div>
        </div>
        
    </div>
</template>

<style lang="scss" scoped>
    #footer-top{
        background-color: #0282f9;
    }
    #footer-center{
        background-image: url('../assets/footer-bg.jpg');
        background-size: cover;
        overflow: hidden;
        .container{
            position: relative;
            
            img{
                position: absolute;
                right: 0;
                top: -6.25rem;
            }
        }
    }
    #footer-bottom{
        background-color: #303030;
        padding: 1.875rem 0;

        button{
            background-color: #303030;
            font-weight: bold;
            border: 2px solid #0282f9;
            padding: .9375rem 1.25rem;
            color: white;
        }
        span{
            color: #0282f9;
            font-weight: bold;
            font-size: 1.0625rem;
        }
    }
</style>