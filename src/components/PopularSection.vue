<template>
    <div class="flex flex-col items-start gap-[24px] h-[42.8125rem] mx-auto m-auto px-[100px]"  id="app">
        <div><p class="font-['Playfair_Display'] text-[#371D1B] text-[40px] leading-[3.3125rem]">Popular Products</p></div>
    <div class="flex gap-[32px] w-[]">
        <div v-for="item of items" v-bind:key="item.id">
            <div class="flex flex-col items-start gap-[24px] h-[38rem]" >
            <div class="w-[24.5rem] h-[28.125rem]">
               <img style="width: 350px; height: 400px;" :src="item.image" />
            </div>
            <div class="flex flex-col items-start gap-[8px]">
                <div class="flex justify-between content-between items-center gap-[210px] w-[24.5rem]">
                    <p class="text">{{ item.title }}</p>
                    <p class="text">{{ item.price }}</p>
                </div>
                <p>{{ item.category }}</p>
            </div>
            <div class="flex justify-center items-center px-px-[20px 32px] border-solid border-2 h-[3.6875rem] w-[24.5rem]">
                <button @click="addToCart(id)" class="text">
                    Add Product to Cart
                </button>
            </div>
        </div>
        </div>
        
    </div>
    </div>
</template>
<script>
import axios from "axios";

export default {
    name: `"PopularSection"`,
    
    data() {
    return {
      items: [],
    };
    },
  
  mounted() {
    this.getStoreData();
  },
  methods: {
    getStoreData() {
      axios
        .get("https://fakestoreapi.com/products")
        .then((response) => {
          this.items = response.data.slice(1, 4);
        })

        .catch((error) => {
          console.log(error);
        });
    },
    addToCart(id) {
      const item = this.itemsInCartIDs.find((item) => item === id);
      console.log(id)
      try {
        if (!item) {
          this.itemsInCartIDs.push(item);
        } else {
        prompt("Product already exists inside the cart.");
        }
      } catch (error) {
        console.log(
          error
        );
      }
    },
  },
}
</script>