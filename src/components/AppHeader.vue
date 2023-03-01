<template>
    <header class="container">
        <div class="menu">
            <img class="logo_header" src="/images/dc-logo.png" alt="">

            <ul class="menu_header">
                <li v-for="menuItem in menuItems" :class="{ 'active': menuItem.active }">
                    {{ menuItem.item }}
                </li>
            </ul>
        </div>
    </header>
</template>

<script>
export default {
    data() {
        return {
            menuItems: [
                { item: 'CHARACTERS' },
                { item: 'COMICS', active: true },
                { item: 'MOVIES' },
                { item: 'TV' },
                { item: 'GAMES' },
                { item: 'COLLECTIBLES' },
                { item: 'VIDEOS' },
                { item: 'FANS' },
                { item: 'NEWS' },
                { item: 'SHOP' },
            ]
        }
    }
}
</script>
  
  <style lang="scss" scoped>

    .menu{
        display: flex;
        justify-content: space-between;
        font-size: 12px;
        font-weight: 600;
        padding: 20px 0;
    }

    .logo_header{
        width: 82px;
    }

    .menu_header{
        display: flex;
        align-items: center;
        gap: 16px;
    }

    .active{
        color: rgba(39,138,249,255);
        position: relative;
    }

    .active::before{
        content: '';
        display: block;
        position: absolute;
        width: 100%;
        height: 5px;
        background-color: rgba(39,138,249,255);
        bottom: -54px;
    }
  
  </style>