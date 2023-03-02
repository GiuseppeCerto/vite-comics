<template>
  <section class="main_section">
    <div class="main_jumbo"></div>
      <div class="bg_color">
        <main class="container">
          <div class="main_ticket">
            CURRENT SERIES
          </div>
          <Card class="card" v-for="(card,i) in cards" :key="i" :series="card.series" :thumb="card.thumb" />
          <div class="main_button">
            LOAD MORE
          </div>
        </main>
      </div>
  </section>
</template>
  
  <script>
    import Card from './Card.vue'
    export default {
      components: {
        Card
      },
      data() {
        return{
          cards: [
            {
              thumb: "/images/img1.jpg",
              price: "$19.99",
              series: "Action Comics",
              type: "comic book"
            },
            {
              thumb: "/images/img2.jpg",
              price: "$3.99",
              series: "American Vampire 1976",
              type: "comic book"
            },
            {
              thumb: "/images/img3.jpg",
              price: "$16.99",
              series: "Aquaman",
              type: "graphic novel"
            },
            {
              thumb: "/images/img4.jpg",
              price: "$2.99",
              series: "Batgirl",
              type: "comic book"
            },
            {
              thumb: "/images/img5.jpg",
              price: "$3.99",
              series: "Batman",
              type: "comic book"
            },
            {
              thumb: "/images/img6.jpg",
              price: "$2.99",
              series: "Batman Beyond",
              type: "comic book"
            },
            {
              thumb: "/images/img7.jpg",
              price: "$3.99",
              series: "Batman/Superman",
              type: "comic book"
            },
            {
              thumb: "/images/img8.jpg",
              price: "$4.99",
              series: "Batman/Superman Annual",
              type: "comic book"
            },
            {
              thumb: "/images/img9.jpg",
              price: "$5.99",
              series: "Batman: The Joker War Zone",
              type: "comic book"
            },
            {
              thumb: "/images/img10.jpg",
              price: "$6.99",
              series: "Batman: Three Jokers",
              type: "comic book"
            },
            {
              thumb: "/images/img11.jpg",
              price: "$4.99",
              series: "Batman: White Knight Presents: Harley Quinn",
              type: "comic book"
            },
            {
              thumb: "/images/img12.jpg",
              price: "$16.99",
              series: "Catwoman",
              type: "graphic novel"
            }
          ]
        }
      }
    }
  </script>
  
  <style lang="scss" scoped>

  .main_jumbo{
    height: 320px;
    background-image: url('/images/jumbotron.jpg');
    background-size: cover;
    background-repeat: no-repeat;
  }

  .bg_color{
    background-color: rgba(28,28,28,255);
  }

  .container{
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    max-width: 1000px;
    font-size: 10px;
    font-weight: 100;
    padding-top: 40px;
    padding-bottom: 40px;
    color: white;
    position: relative;
    justify-content: center;
  }
  .card{
    flex-basis: calc(100% / 6 - 53px / 6);
  }

  .main_ticket{
    position: absolute;
    background-color: rgba(2,130,249,255);
    padding: 10px 20px;
    font-size: 15px;
    font-weight: 600;
    top: -20px;
    left: 0;
  }

  .main_button{
    background-color: rgba(2,130,249,255);
    padding: 10px 40px;
    font-size: 15px;
    font-weight: 600;
    justify-self: center;
    margin-top: 20px;
  }
  </style>