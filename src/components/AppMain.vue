<template>
  <section class="main_section">
    <div class="main_jumbo"></div>
      <main class="container">
        <Card class="card" v-for="(card,i) in cards" :key="i" :series="cards.series" :thumb="card.thumb" />
      </main>
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
              thumb: "/image/img1",
              price: "$19.99",
              series: "Action Comics",
              type: "comic book"
            },
            {
              thumb: "/image/img2",
              price: "$3.99",
              series: "American Vampire 1976",
              type: "comic book"
            },
            {
              thumb: "/image/img3",
              price: "$16.99",
              series: "Aquaman",
              type: "graphic novel"
            },
            {
              thumb: "/image/img4",
              price: "$2.99",
              series: "Batgirl",
              type: "comic book"
            },
            {
              thumb: "/image/img5",
              price: "$3.99",
              series: "Batman",
              type: "comic book"
            },
            {
              thumb: "/image/img6",
              price: "$2.99",
              series: "Batman Beyond",
              type: "comic book"
            },
            {
              thumb: "/image/img7",
              price: "$3.99",
              series: "Batman/Superman",
              type: "comic book"
            },
            {
              thumb: "/image/img8",
              price: "$4.99",
              series: "Batman/Superman Annual",
              type: "comic book"
            },
            {
              thumb: "/image/img9",
              price: "$5.99",
              series: "Batman: The Joker War Zone",
              type: "comic book"
            },
            {
              thumb: "/image/img10",
              price: "$6.99",
              series: "Batman: Three Jokers",
              type: "comic book"
            },
            {
              thumb: "/image/img11",
              price: "$4.99",
              series: "Batman: White Knight Presents: Harley Quinn",
              type: "comic book"
            },
            {
              thumb: "/image/img12",
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

  .container{
    display: flex;
  }
  .card{
    flex-basis: calc(100% / 6);
  }
  </style>