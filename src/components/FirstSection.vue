<template>
  <div>
    <div class="flex flex-col items-start relative font-sans">
      <img class="" src="../assets/FirstSection.png" />
      <div
        class="absolute h-[16.8125rem] w-[40.375rem] top-[240px] left-[135px]"
      >
        <p class="font-normal text-6xl not-italic text-[#371D1B]">
          DISCOVER UNIQUE & AUTHENTIC WEARS
        </p>
        <button
          class="bg-[#3D3939] text-[#FEE9D8] hover:bg-[#FEE9D8] hover:text-[#3D3939] border-2 border-[#3D3939] w-[130px] h-[50px] mt-8"
        >
          Discover Now
        </button>
      </div>
    </div>
    <Logo />
  </div>
</template>

<script>
import Logo from "./Logo";
export default {
  name: `"FirstSection"`,
  components: {
    Logo,
  },
};
</script>
