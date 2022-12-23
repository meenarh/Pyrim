<template>
  <div
    class="flex flex-col items-start gap-[24px] h-[100.8125rem] mx-auto m-auto px-[100px]"
  >
    <div>
      <p class="font-['Playfair_Display'] text-[#371D1B] text-[40px]">
        Best Selling Products
      </p>
    </div>
    <div class="grid grid-cols-3 gap-[32px]">
      <div v-for="item of items" v-bind:key="item.id">
        <div>
          <div class="flex flex-col items-start gap-[24px] h-[50rem]">
            <div class="w-[24.5rem] h-[30.125rem]">
              <img style="width: 350px; height: 400px;" class="mt-10" :src="item.image" />
            </div>
            <div class="flex flex-col items-start gap-[8px] h-[5rem]">
              <div
                class="flex justify-between content-between items-center gap-[130px] w-[24.5rem] h-[3.6875rem]]"
              >
                <p class="text">{{ item.title }}</p>
                <p class="text">{{ realPrice(item.price) }}</p>
              </div>
              <p>{{ item.category }}</p>
            </div>
            <div
              class="flex justify-center items-center px-[32px] border-solid border-2 h-[3.6875rem] w-[24.5rem]"
            >
              <button @click="addToCart(item.id)" class="text">Add Product to Cart</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";

export default {
  name: `"BestSellingSection"`,
  data() {
    return {
      items: [],
      itemsInCartIDs: [],
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
          this.items = response.data.slice(1, 5);
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
    realPrice(oldPrice) {
      return oldPrice * 1.022;
    },
  },
};
</script>
