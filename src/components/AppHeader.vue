<script>
    import AppLogo from './AppLogo.vue';
    import AppPrimaryNav from './AppPrimaryNav.vue';
    export default {
        name: 'AppHeader', 
        components: {
            AppLogo, 
            AppPrimaryNav
        }
    }
</script>

<template>
    <div class="container flex space-between">
        <AppLogo/>
        <AppPrimaryNav/>
    </div>
</template>

<style scoped>

</style>