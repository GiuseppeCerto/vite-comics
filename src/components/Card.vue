<template>
    <li class="card">
      <img :src="thumb" alt="">
      <h3 class="card_title">{{ series }}</h3>
    </li>
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

  
  </style>