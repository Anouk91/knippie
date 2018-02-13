<template>

  <div style="padding-top: 2rem" class="imageGrid">
    <b-button :pressed.sync="button" variant="outline-secondary sm">In Stock</b-button>
    <div class="products">
      <div v-for="card in filteredList"  :key="card.id" >
        <div class="card"  v-bind:style='{ backgroundImage: "url(" + card.image + ")", }'>
          <div  v-if="active" class="cardText" display="block"></div>   <!-- {{card.stock}} -->
        </div>
          <!-- <b-modal id="modal1" title="Bootstrap-Vue">
    <p class="my-4">Hello from modal!</p>
  </b-modal> -->
      </div>
    </div>
  </div>

</template>
  
<script>
import canCards from '../canCards'
export default {
  data () {
    return {
      button: false,
      instock: false,
      sold: false,
      active: true,
      canCards
    }
  },
  computed: {
    filteredList () {
      if (this.button) {
        return this.canCards.filter(c => c.stock > 0)
      } else {
        return this.canCards
      }
    }
  }
  // },
  // method: {
  //   change: fuction()
  // }
}
</script>

<style>
.imageGrid {
  background-color: #d6e0f5;
}
.products {
  display: flex;
  max-width: textwidth;
  flex-wrap: wrap;
  padding-top: 12px;
  padding-bottom: 12px;
  /* background-color: gray; */
}

.card {
  width: 100px;
  height: 100px;
  margin: 12px;
  position: relative;

  background-size: 100px 100px;
}

.cardText {
  position: absolute;
  bottom: 0;
  right: 0;
  margin-right: 2px;
  font-weight: bold;
}
</style>