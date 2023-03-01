<template>
    <header class="container">
        <div class="menu">
            <img class="logo_header" src="/images/dc-logo.png" alt="">

            <ul class="menu_header">
                <li>characters</li>
                <li>comics</li>
                <li>movies</li>
                <li>tv</li>
                <li>games</li>
                <li>collectibles</li>
                <li>videos</li>
                <li>fans</li>
                <li>news</li>
                <li>shop</li>
            </ul>
        </div>
    </header>
  </template>
  
  <script>
    export default {
      
    }
  </script>
  
  <style lang="scss" scoped>
    .logo_header{
        width: 82px;
    }

    .menu{
        display: flex;
        gap: 470px;
    }

    .menu_header{
        display: flex;
        align-items: center;
        gap: 30px;
    }
  
  </style>