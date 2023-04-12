<script>
import JumbotronItem from "./JumbotronItem.vue";
import NavbarItem from "./NavbarItem.vue"
 export default {
    name: 'Header',
    data() {
        return {
            
        }
    },
    components:{
    NavbarItem,
    JumbotronItem
}
 }
</script>

<template>
    <NavbarItem></NavbarItem>
    <JumbotronItem></JumbotronItem>
</template>

<style scoped>

</style>
