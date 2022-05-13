<template>
  <header class="container">
    <div class="logo">
        <img src="../assets/img/dc-logo.png" alt="">
    </div>
    <nav class="h-100">
        <ul class="h-100">
            <li v-for="(item,index) in itemsMenu" :key="`menu-${index}`">
                <a :class="{'active' : item.isActive}" :href="item.href">{{item.name}}</a>
            </li>
        </ul>
    </nav>
  </header>
</template>

<script>
export default {
    name: 'HeaderComponent',

    data(){
        return{
            itemsMenu: [
                {
                    name: 'Characters',
                    href: '#',
                    isActive: false
                },
                {
                    name: 'Comics',
                    href: '#',
                    isActive: true
                },
                {
                    name: 'Movies',
                    href: '#',
                    isActive: false
                },
                {
                    name: 'Tv',
                    href: '#',
                    isActive: false
                },
                {
                    name: 'Games',
                    href: '#',
                    isActive: false
                },
                {
                    name: 'Collectibles',
                    href: '#',
                    isActive: false
                },
                {
                    name: 'Videos',
                    href: '#',
                    isActive: false
                },
                {
                    name: 'Fans',
                    href: '#',
                    isActive: false
                },
                {
                    name: 'News',
                    href: '#',
                    isActive: false
                },
                {
                    name: 'Shop',
                    href: '#',
                    isActive: false
                },
                
            ]
        }
    }
}
</script>

<style lang="scss" scoped>

@import "../assets/style/mixins";
@import "../assets/style/vars";

header{
    height: 120px;
    @include header-menu();
    .logo img{
    width: 80px;
    }
    nav{
        ul{
        display: flex;
        }
        li{
        display: flex;       
        }
        a{
        padding: 0 10px ;
        color: black;
        line-height: 110px;
        text-transform: uppercase;
        font-size: .8rem;
        &:hover,
        &.active{
            color: $brand-color;
            border-bottom: 3px solid $brand-color;
        }
        }
    }
    
    

}
</style>