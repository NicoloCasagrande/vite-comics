<script>
    export default {
        name: 'AppPrimaryNav', 
        data(){
            return{
                activeMenu: 0, 
                menuChoice: [
                    {   
                        href: '#', 
                        label: 'CHARACTERS', 
                        active: true
                    },
                    {   
                        href: '#', 
                        label: 'COMICS', 
                        active: false
                    },
                    {   
                        href: '#', 
                        label: 'MOVIES', 
                        active: false
                    },
                    {   
                        href: '#', 
                        label: 'TV', 
                        active: false
                    },
                    {   
                        href: '#', 
                        label: 'GAMES', 
                        active: false
                    },
                    {   
                        href: '#', 
                        label: 'COLLECTIBLES', 
                        active: false
                    },
                    {   
                        href: '#', 
                        label: 'VIDEOS', 
                        active: false
                    },
                    {   
                        href: '#', 
                        label: 'FANS', 
                        active: false
                    },
                    {   
                        href: '#', 
                        label: 'NEWS', 
                        active: false
                    },
                    {   
                        href: '#', 
                        label: 'SHOP', 
                        active: false
                    }
                ]
            }
        }, 
        methods: {
            changeLink(index){
                this.menuChoice.forEach((element, i) => {
                    console.log(element);
                    if(i === index){
                        element.active = true;
                        this.menuChoice[this.activeMenu].active = false;
                        this.activeMenu = i;
                    }else{
                        
                    }
                });
            }
        }
    }
</script>

<template>
    <nav>
        <ul>
            <li v-for="(choice, index) in menuChoice"><a :class= "choice.active ? 'active': ''" href="" @click="changeLink(index)">{{choice.label}}</a></li>
        </ul>
    </nav>
</template>

<style lang="scss" scoped>
    .active{
        color: var(--primary-color);
    }
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
                color: black;
                &:hover{
                    color: var(--primary-color);
                    cursor: pointer;
                }
            }
        }
    }
</style>