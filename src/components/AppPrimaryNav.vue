<script>
    export default {
        name: 'AppPrimaryNav'
    }
</script>

<template>
    <nav>
        <ul>
            <li><a href="">CHARACTERS</a></li>
            <li><a href="">COMICS</a></li>
            <li><a href="">MOVIES</a></li>
            <li><a href="">TV</a></li>
            <li><a href="">GAMES</a></li>
            <li><a href="">COLLECTIBLES</a></li>
            <li><a href="">VIDEOS</a></li>
            <li><a href="">FANS</a></li>
            <li><a href="">NEWS</a></li>
            <li><a href="">SHOP</a></li>
        </ul>
    </nav>
</template>

<style lang="scss" scoped>
    nav {
        ul {
            display: flex;
            list-style: none;
            justify-content: center;
            align-items: center;

            a{
                text-decoration: none;
                margin-left: 1.25rem;
                font-weight: bold;
            }
        }
    }
</style>