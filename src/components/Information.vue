<template>
  <div class="infomation">
    <b-carousel id="carousel1"
                style="text-shadow: 1px 1px 2px #669900;"
                controls
                indicators
                background="#f2f2f2"
                :interval="4000"
                img-width="1024"
                img-height="400px"
                v-model="slide"
                @sliding-start="onSlideStart"
                @sliding-end="onSlideEnd"
    >

      <!-- Text slides with image -->
      <b-carousel-slide caption=""
                        text=""
                        img-src=  "/static/menu/types.png"
      ></b-carousel-slide>

      <b-carousel-slide caption=""
                        text=""
                        img-src=  "/static/menu/made.png"
      ></b-carousel-slide>
      <b-carousel-slide caption=""
                        text=""
                        img-src=  "/static/menu/size.png"
      ></b-carousel-slide>


    </b-carousel>

    <h1 style="margin-top: 2rem;">KNIPPIE</h1> 
    <h3 style="font-style: italic;"> The Upcycled Cheerful Protective Cardholder </h3>
    <b-row class="features">
      <b-col class="feature">
        <div class="title">
        Scam Protected
        </div>
        <div>
           The aluminium front and back of the wallet protect your RFID cards from scamming.
        </div>
      </b-col>
      <b-col class="feature">      
        <div class="title">
          Recycled
        </div>
        <div>
          The front of the wallet is made out of old can  + a misprinted plastic business card.
        </div>
      </b-col>
      </b-row>
    <b-row class="features">
      <b-col class="feature">      
      <div class="title">
        Super Slim
        </div>
        <div>
          Knippie adjusts itself to the amount of cards it has to protect.
        </div>
      </b-col>
      <b-col class="feature">      
      <div class="title">
        Unique
        </div>
        <div>
          Every Knippie is handmade out of a old can, and is therefore always 100% unique to its peers. You can even bring in your own favourite can!
        </div>
      </b-col>
    </b-row>
    <b-row class="video">
      <div class="title" > Easy to use!</div>
      <div> A Knippie is like a deck of cards. Just fold it open and thumb through. </div>
    <video width="320" height="240" style="margin-top: 2rem;" autoplay loop>
    <source src="/static/menu/usage.mp4" type="video/mp4">
    Your browser does not support the video tag.
    </video> 
</b-row>
  </div>
</template>


<script>
// import menu from "../menu";
// export default {
//   data() {
//     return {
//       selected: menu[0],
//       menu
//     };
//   }
// };
</script>


<style>

.video {
  margin-top: 2rem;
  display: inline-block;
  align-content: middle;
}

.features {
  margin-left: 5rem;
}

.features > b-col {
  display: flex;
  flex-wrap: wrap;
}


.feature{
  padding-top: 2rem;
  margin-right: 5rem;
}
.title {
  font-weight: bold;
}



</style>
