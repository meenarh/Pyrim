<template>
  <div class="bg-[#211212] w-[1440px] h-[408px] flex flex-col font-sans text-center pt-8">
    <div class="p-4">
      <h3 class="text-2xl text-white font-normal capitalize p-2">
        Subscribe to our newsletter
      </h3>
      <p class="text-sm text-[#F2ECE6] font-normal">
        Get all the latest information on events, sales and offers.
      </p>
    </div>
    <div class="p-4">
      <input
        class="p-3 bg-[#42302F] w-[492px] h-[60px] text-white font-normal text-sm]"
        type="email"
        placeholder="Enter your email"
      />
      <button class="bg-[#FEE9D8] w-[132px] h-[60px] hover:bg-[#211212] hover:text-[#FEE9D8] hover:border" style="border-radius: 2px;">Subscribe</button>
    </div>
    <div class="flex flex-row p-8 ml-10 mr-14 justify-between">
      <div class="socials flex flex-row gap-10">
         <img src="../assets/twitter.png" alt="Twitter" />
         <img src="../assets/instagram.png" alt="Instagram" />
         <img src="../assets/whatsapp.png" alt="WhatsApp" />
      </div>
         <ul class="list-none flex flex-row gap-10 text-white text-sm font-normal">
            <li>About</li>
            <li>Contact</li>
            <li>FAQs</li>
            <li>Blog</li>
            <li>Privacy</li>
            <li>Terms</li>
         </ul>
    </div>
    <div>
      <p class="text-sm text-[#908888] font-normal">
        © 2022 Pyrim. All Rights Reserved.
      </p>
    </div>
  </div>
</template>
<script>
export default {
  name: `"Footer"`,
};
</script>
<style lang=""></style>
