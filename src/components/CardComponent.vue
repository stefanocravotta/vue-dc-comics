<template>
  <div class="card">
      <div class="container-img">
          <img :src="comic.thumb" :alt="comic.type">
      </div>
      
      <h3>{{comic.series}}</h3>
  </div>
</template>

<script>
export default {
    name: 'CardComponent',
    props:{
        comic:Object,
    }

}
</script>

<style lang="scss" scoped>

.card{
        flex-basis: calc(100% / 6 - 20px);
        height: 250px;
        overflow: hidden;
        margin: 0 10px;
        color: white;
        .container-img{
            height: 70%;
            overflow: hidden;
        }
        h3{
            margin-top: 15px;
            font-size: 1rem;
        }
    }

</style>