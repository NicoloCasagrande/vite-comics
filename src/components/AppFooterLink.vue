<script>
    export default {
        name: 'AppFooterLink', 
        data(){
            return{
                    list:[
                    {
                        name: 'DC COMICS',
                        informations: [
                            'Characters', 
                            'Comics',
                            'Movies', 
                            'TV', 
                            'Games', 
                            'Videos', 
                            'News'
                        ]
                    },
                    {
                        name: 'SHOP', 
                        informations: [
                            'Shop DC', 
                            'Shop DC Collectibles'
                        ]
                    }, 
                    {
                        name: 'DC',
                        informations: [
                            'Terms of Use', 
                            'Privacy policy (New)', 
                            'Ad Choices', 
                            'Advertising', 
                            'Jobs', 
                            'Subscriptions', 
                            'Talent Workshops', 
                            'CPSC Certificates', 
                            'Ratings', 
                            'Shop Help', 
                            'Contact Us'
                        ]
                    }, 
                    {
                        name: 'SITES', 
                        informations: [
                            'DC',
                            'MAD Magazine', 
                            'DC Kids', 
                            'DC Universe', 
                            'DC Power Visa'
                        ]
                    }
                ]
            }
        }
    }
</script>

<template>
    <div class="flex column flex-wrap height-c-footer">
        <div v-for="onelist in list" class="flex column flex-wrap margin-ten">
            <h3>{{onelist.name}}</h3>
            <span v-for="information in onelist.informations">{{information}}</span>
        </div>
    </div>
</template>

<style scoped>
    h3{
        display: inline;
        padding: .625rem 0;
        font-size: 1.25rem;
        font-weight: bold;
    }
    span{
        padding: 2px 0;
        color: gray;
    }
    .height-c-footer{
        height: 21.875rem;
        width: 30%;
        padding: 1.25rem;
    }
    .margin-ten{
        margin-right: 1.25rem;
    }
</style>