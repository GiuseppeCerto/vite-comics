<template>
    <div class="card">
      <img class="img_card" :src="thumb" alt="">
      <h3 class="card_title">{{ series }}</h3>
    </div>
</template>
  
<script>
    export default {
      props: {
        thumb: String,
        series: String,
      }
    }
</script>
  
<style lang="scss" scoped>
  @use '../style/partials/variables' as *;

  .img_card{
    width: 150px;
  }

  .card_title{
    margin-top: 7px;
  }

  
</style>