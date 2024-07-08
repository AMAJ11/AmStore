<template>
  <v-app class="pt-5"
    ><div class="pt-16">
      <v-carousel
        show-arrows="hover"
        cycle
        interval="2000"
        hide-delimiter-background="true"
      >
        <v-carousel-item
          cover
          src="../assets/pexels-laurachouette-21263377.jpg"
        >
          <div
            class="div"
            style="width: 70%; padding-left: 10%; padding-top: 20%"
          >
            <h2>Iphone</h2>
            <p class="text-black w-75">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
              Nostrum,ipsum dolor sit amet consectetur adipisicing elit.
            </p>
            <v-btn color="success" variant="outlined" class="mt-5"
              >Buy now</v-btn
            >
          </div>
        </v-carousel-item>
        <v-carousel-item cover src="../assets/pexels-veeterzy-303383.jpg">
          <div style="width: 70%; padding-left: 10%; padding-top: 20%">
            <h2>Macbook</h2>
            <p class="text-white w-75">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
              Nostrum,ipsum dolor sit amet consectetur adipisicing elit.
            </p>
            <v-btn color="success" variant="outlined" class="mt-5"
              >Buy now</v-btn
            >
          </div></v-carousel-item
        >
        <v-carousel-item
          cover
          src="../assets/pexels-dina-nasyrova-2006209-3825517.jpg"
        >
          <div style="width: 70%; padding-left: 10%; padding-top: 20%">
            <h2>Airpods</h2>
            <p class="text-black w-75">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
              Nostrum,?ipsum dolor sit amet consectetur adipisicing elit.
            </p>
            <v-btn color="success" variant="outlined" class="mt-5"
              >Buy now</v-btn
            >
          </div></v-carousel-item
        >
        <v-carousel-item cover src="../assets/pexels-tdcat-437037.jpg">
          <div style="width: 70%; padding-left: 10%; padding-top: 20%">
            <h2 class="text-white">Smart watch</h2>
            <p class="text-white w-75">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
              Nostrum,ipsum dolor sit amet consectetur adipisicing elit.
            </p>
            <v-btn color="success" variant="outlined" class="mt-5"
              >Buy now</v-btn
            >
          </div></v-carousel-item
        >
        <v-carousel-item
          cover
          src="../assets/pexels-webber-amir-1551084-20348034.jpg"
        >
          <div style="width: 70%; padding-left: 10%; padding-top: 20%">
            <h2>Samsung s24 ultra</h2>
            <p class="text-black w-75">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
              Nostrum,ipsum dolor sit amet consectetur adipisicing elit.
            </p>
            <v-btn color="success" variant="outlined" class="mt-5"
              >Buy now</v-btn
            >
          </div></v-carousel-item
        >
      </v-carousel>
    </div>
    <div class="pop mt-10 px-5 d-flex">
      <h2>Populer product</h2>
      <v-spacer></v-spacer>
      <span>
        <v-btn color="success" variant="text"
          ><v-icon>mdi-arrow-left</v-icon></v-btn
        ><v-btn color="success" variant="text"
          ><v-icon>mdi-arrow-right</v-icon></v-btn
        >
      </span>
    </div>
    <v-container>
      <v-row>
        <v-col
          cols="12"
          sm="6"
          md="6"
          lg="3"
          xl="3"
          v-for="n in this.popprod"
          :key="n"
        >
          <v-card
            variant="tonal"
            data-aos="fade-right"
            data-aos-duration="1000"
          >
            <img class="im" :src="n.src" style="height: 200px; width: 100%" />
            <v-card-text>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Quod
              alias, error aperiam obcaecati fugiat quo adipisci facere
              molestias eum ex accusantium qui praesentium quae temporibus, sit
              reprehenderit blanditiis, dolores eos!
            </v-card-text>
            <v-card-actions>
              <v-rating
                size="xsm"
                hover
                color="warning"
                half-increments
              ></v-rating
              ><v-spacer></v-spacer>
              <p class="text-success">{{ n.price }}$</p>
            </v-card-actions>
            <v-btn variant="outlined" class="mx-3" color="success">Buy</v-btn>
            <v-btn variant="outlined" color="warning">Info</v-btn>
          </v-card>
        </v-col>
      </v-row>
    </v-container>

    ///////////////////////////////////////////////////

    <v-divider></v-divider>

    <div class="pop mt-10 px-5 d-flex">
      <h2>Featured Products</h2>
      <v-spacer></v-spacer>
      <span>
        <v-btn color="success" variant="text"
          ><v-icon>mdi-arrow-left</v-icon></v-btn
        ><v-btn color="success" variant="text"
          ><v-icon>mdi-arrow-right</v-icon></v-btn
        >
      </span>
    </div>
    <v-container>
      <v-row>
        <v-col
          cols="12"
          sm="6"
          md="6"
          lg="3"
          xl="3"
          v-for="n in this.featprod"
          :key="n"
        >
          <v-card
            variant="tonal"
            data-aos="flip-right"
            data-aos-duration="1000"
          >
            <img class="im" :src="n.src" style="height: 200px; width: 100%" />
            <v-card-text>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Quod
              alias, error aperiam obcaecati fugiat quo adipisci facere
              molestias eum ex accusantium qui praesentium quae temporibus, sit
              reprehenderit blanditiis, dolores eos!
            </v-card-text>
            <v-card-actions>
              <v-rating
                size="xsm"
                hover
                color="warning"
                half-increments
              ></v-rating
              ><v-spacer></v-spacer>
              <p class="text-success">{{ n.price }}$</p>
            </v-card-actions>
            <v-btn variant="outlined" class="mx-3" color="success">Buy</v-btn>
            <v-btn variant="outlined" color="warning">Info</v-btn>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
    <v-container>
      <div class="py-12 px-16 mt-5 bg-grey-lighten-3">
        <h2 class="text-center">Offer expiration time</h2>
        <h1 class="text-center text-success">12:58:10</h1>
        <v-row>
          <v-col cols="12" lg="6" v-for="n in this.offer" :key="n">
            <v-card variant="outlined" class="bg-white">
              <img :src="n.src" alt="" />
              <v-card-actions class="bg-warning">
                <h3 style="text-decoration: line-through">{{ n.oprice }}$</h3>
                <h2 class="text-black ml-6">{{ n.nprice }}$</h2>
              </v-card-actions>
            </v-card>
          </v-col>
        </v-row>
      </div>
    </v-container>
    <v-container>
      <h1>News</h1>
      <div class="pa-16 bg-grey-lighten-2">
        <v-row>
          <v-col cols="12" lg="3" v-for="num in this.news" :key="num">
            <v-card>
              <v-card-title primary-title> {{ num.title }} </v-card-title>
              <img style="width: 100%; height: 300px" :src="num.src" alt="" />
            </v-card>
          </v-col>
        </v-row>
      </div>
    </v-container>

    <div class="mt-6 bg-black pa-15">
      <v-row>
        <v-col cols="12" lg="6">
          <h2 class="text-blue">AM store</h2>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Nostrum
            reprehenderit tempora distinctio nisi iste veritatis veniam delectus
            nihil recusandae accusantium. Animi exercitationem magnam
            doloremque, hic illum explicabo amet vero qui!
          </p>
        </v-col>
        <v-col cols="12" lg="2" md="6">
          <h3 class="text-blue">About</h3>
          <a class="mt-3" href="..." style="text-decoration: none; color: gray"
            >how We work </a
          ><br />
          <a class="mt-3" href="..." style="text-decoration: none; color: gray"
            >how We work </a
          ><br />
          <a class="mt-3" href="..." style="text-decoration: none; color: gray"
            >how We work </a
          ><br />
          <a class="mt-3" href="..." style="text-decoration: none; color: gray"
            >how We work </a
          ><br />
          <a class="mt-3" href="..." style="text-decoration: none; color: gray"
            >how We work
          </a>
        </v-col>
        <v-col cols="12" lg="2" md="6">
          <h3 class="text-blue">more Services</h3>
          <p class="mt-3">dilevary for all world</p>
          <p class="mt-3">dilevary for all world</p>
          <p class="mt-3">dilevary for all world</p>
          <p class="mt-3">dilevary for all world</p>
        </v-col>
        <v-col cols="12" lg="2" md="6">
          <h3 class="text-blue">more Services</h3>
          <p class="mt-3">dilevary for all world</p>
          <p class="mt-3">dilevary for all world</p>
          <p class="mt-3">dilevary for all world</p>
          <p class="mt-3">dilevary for all world</p>
        </v-col>
      </v-row>
    </div>
  </v-app>
</template>

<script>
export default {
  name: "index",
  components: {},
  data: function () {
    return {
      popprod: [
        {
          src: "https://m.media-amazon.com/images/I/611Ikj0gCSL._AC_UY218_.jpg",
          price: "450.5",
        },
        {
          src: "https://m.media-amazon.com/images/I/51KCV2cdDsS._AC_UY218_.jpg",
          price: "79",
        },
        {
          src: "https://m.media-amazon.com/images/I/51m9FoHWpcL._AC_UY218_.jpg",
          price: "113.7",
        },
        {
          src: "https://m.media-amazon.com/images/I/71KbTAWLTNL._AC_UY218_.jpg",
          price: "152",
        },
      ],
      featprod: [
        {
          src: "https://m.media-amazon.com/images/I/51fM0CKG+HL._AC_UY218_.jpg",
          price: "2354",
        },
        {
          src: "https://m.media-amazon.com/images/I/71Blu2gkgnL._AC_UY218_.jpg",
          price: "1897",
        },
        {
          src: "https://m.media-amazon.com/images/I/71vYeYqdvUL._AC_UY218_.jpg",
          price: "2136",
        },
        {
          src: "https://m.media-amazon.com/images/I/71xaNEUxYML._AC_UY218_.jpg",
          price: "756",
        },
      ],
      offer: [
        {
          src: "https://m.media-amazon.com/images/I/81Dm65eja8L._AC_UY218_.jpg",
          oprice: "231",
          nprice: "189",
        },
        {
          src: "https://m.media-amazon.com/images/I/51-X+HBW4JL._AC_UY218_.jpg",
          oprice: "101",
          nprice: "72",
        },
      ],
      news: [
        {
          src: "https://m.media-amazon.com/images/I/61afOyd+zEL._AC_UY218_.jpg",
          title: "Iphone 15 pro max",
        },
        {
          src: "https://m.media-amazon.com/images/I/61D2-aWW4hL._AC_UY218_.jpg",
          title: "Airpods case",
        },
        {
          src: "https://m.media-amazon.com/images/I/81SkpwyPZnL._AC_UL320_.jpg",
          title: "New microphone",
        },
        {
          src: "https://m.media-amazon.com/images/I/71GMtNr13QL._AC_UY218_.jpg",
          title: "Laptop stand",
        },
      ],
    };
  },
  methods: {},
};
</script>

<style scoped></style>
