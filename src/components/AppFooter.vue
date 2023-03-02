<template>
  <footer>
    <section class="footer_section_1">
      <div class="container main_menu_footer">
        <div class="link_container">
          <img class="bg_logo" src="/images/dc-logo-bg.png" alt="">
          <ul>
            <li v-for="DcComicsItem in DcComicsItems" :class="{ 'list_title': DcComicsItem.list_title }">
              {{ DcComicsItem.item }}
            </li>
          </ul>

          <ul>
            <li v-for="DcShopItem in DcShopItems" :class="{ 'list_title': DcShopItem.list_title }">
              {{ DcShopItem.item }}
            </li>
          </ul>
        </div>

        <div class="link_container">
          <ul>
            <li v-for="DcItem in DcItems" :class="{ 'list_title': DcItem.list_title }">
              {{ DcItem.item }}
            </li>
          </ul>
        </div>
        <div class="link_container">
          <ul>
            <li v-for="SitesItem in SitesItems" :class="{ 'list_title': SitesItem.list_title }">
              {{ SitesItem.item }}
            </li>
          </ul>
        </div>
      </div>
    </section>

    <section class="footer_section_2">
      <div class="container main_menu_footer_2">
        <div class="footer_button">
          <span>SIGN-UP NOW!</span>
        </div>
        <div class="follow_link">
          <span>FOLLOW US</span>
          <img src="/images/footer-facebook.png" alt="">
          <img src="/images/footer-twitter.png" alt="">
          <img src="/images/footer-youtube.png" alt="">
          <img src="/images/footer-pinterest.png" alt="">
          <img src="/images/footer-periscope.png" alt="">
        </div>
      </div>
    </section>
  </footer>
  </template>
  
  <script>
  export default {
      data() {
          return {
              DcComicsItems: [
                { item: 'DC COMICS', list_title: true },
                { item: 'Characters'},
                { item: 'Comics' },
                { item: 'Movies' },
                { item: 'Tv' },
                { item: 'Games' },
                { item: 'Videos' },
                { item: 'News' },
              ],
              DcShopItems: [
                { item: 'SHOP', list_title: true },
                { item: 'Shop DC'},
                { item: 'Shop DC Collectibles' },
              ],
              DcItems: [
                { item: 'DC', list_title: true },
                { item: 'Terms of Use'},
                { item: 'Privacy Policy (New)' },
                { item: 'Ad Choices' },
                { item: 'Advertising' },
                { item: 'Jobs' },
                { item: 'Subscription' },
                { item: 'Talent Workshops' },
                { item: 'CPSC Cerfificates' },
                { item: 'Ratings' },
                { item: 'Shop Help' },
                { item: 'Contact Us' },
              ],
              SitesItems: [
                { item: 'SITES', list_title: true },
                { item: 'MAD Megazine'},
                { item: 'DC Kids' },
                { item: 'DC Universe' },
                { item: 'DC Power Visa' },
              ],
          }
      }
  }
  </script>
  
  <style lang="scss" scoped>
    .footer_section_1{
      background-image: url('/images/footer-bg.jpg');
      background-repeat: no-repeat;
      background-size: cover;
      position: relative;
    }

    .main_menu_footer{
      display: flex;
    }

    .link_container{
      margin: 45px 45px 35px 0;
    }

    .bg_logo{
      width: 480px;
      position: absolute;
      bottom: -30px;
      right: 200px;
    }

    .link_container li{
      font-size: 13px;
      color: rgba(111,124,135,255);
      margin-bottom: 4px;
    }

    .link_container ul{
      margin-bottom: 30px;
    }

    .list_title{
      font-weight: 600;
      font-size: 20px !important;
      margin-bottom: 15px !important;
      color: white !important;
    }

    .footer_section_2{
      background-color: rgba(48,48,48,255);
      position: relative;
      z-index: 10;
      padding: 30px 0;
    }

    .main_menu_footer_2{
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .footer_button{
      color: white;
      padding: 10px;
      border: 2px solid rgba(2,130,249,255);
      font-size: 13px;
    }

    .follow_link{
      display: flex;
      align-items: center;
      gap: 15px;
    }

    .follow_link span{
      color: rgba(2,130,249,255);
      font-size: 18px;
      font-weight: 600;
      align-self: center;
    }

    .follow_link img{
      width: 28px;
    }
  
  </style>