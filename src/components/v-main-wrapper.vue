<template>
    <div class="v-main-wrapper">

      <div> <v-catalog/></div>
            <v-cart/>

    </div>
</template>
<script>
    import vCatalog from './v-catalog'
    import vCart from './v-cart'
    export default{
        name: 'v-main-wrapper',
        components:{
          vCatalog,vCart
        },
        props:{},
        data(){
            return{
                title:'Main wrapper'
            }
        },
        computed:{},
        methods:{},
        watch:{},
        mounted(){
            
        }
    }
</script>
<style scoped>
    .v-main-wrapper{

        max-width: 500px;
        margin: 0 auto;
    }
</style>