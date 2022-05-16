<template>
  <main>
      <div class="jumbotron"></div>
      <div class="container card-container">

        <button class="btn">CURRENT SERIES</button>
        
        <CardComponent
        v-for="(comicItem,index) in DcComics"
        :key="`comic-${index}`"
        :comic="comicItem"
        class="card" />

      </div>
      <button class="btn-load">LOAD MORE</button>
      
  </main>
</template>

<script>
import DcComics from '../assets/data/DcComics';
import CardComponent from './CardComponent.vue';

export default {
    name: 'MainComponent',
    components : {
    CardComponent,
},
    data(){
        return{
            DcComics
        }
    },
    mounted() {
        console.log(this.DcComics);
    },
}
</script>

<style lang="scss" scoped>

@import "../assets/style/vars";
@import "../assets/style/mixins";


main{
    background-color: #1c1c1c;
    text-align: center;
    .jumbotron{
    height: 400px;
    background-image: url(../assets/img/jumbotron.jpg);
    background-position:initial;
    background-size: cover;
    }
    .card-container{
    display: flex;
    position: relative;
    flex-wrap: wrap;
    padding: 40px 0;
    .btn{
        position: absolute;
        top: -15px;
        left: 0;
        @include btn();
        border: none;
        background-color: $brand-color;
        }
    }
    .btn-load{
        @include btn();
        border: none;
        background-color: $brand-color;
        padding: 10px 50px;
        margin: 15px 0;
    }
}

</style>