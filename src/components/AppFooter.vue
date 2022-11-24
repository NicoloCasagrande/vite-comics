<script>
    import AppCard from './AppCard.vue';
    export default {
        name: 'AppFooter', 
        components: {
            AppCard
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
        <div class="flex column">
            
        </div>
    </div>
    <div class="footer-bottom flex">
        
    </div>
</template>

<style scoped>
    #footer-top{
        background-color: #0282f9;
    }
    #footer-center{
        background-image: url('../assets/footer-bg.jpg');
    }
</style>