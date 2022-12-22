<template>
    <div class="bg-[#3D3939] flex items-center h-[6.25rem] justify-around font-sans">
        <div class="flex items-center gap-[0.5rem] w-[6.25rem]">
            <SvgComponent />
            <span class="text-white uppercase">Pyrim</span>
        </div>
        <div class="flex gap-[2.5rem] text-white">
            <p>Trending</p>
            <p>Product</p>
            <p>For Men</p>
            <p>For Women</p>
            <p>For Kids</p>
        </div>

        <div class="flex w-[5.0625rem] gap-[0.5rem]">
            <p class="text-white pt-2">Cart</p>
            <div class="bg-[#ffffff] w-[2.5rem] h-[2.5rem] flex justify-center items-center text-lg">0</div>
        </div>
    </div>
</template>

<script>
import SvgComponent from './SvgComponent';
export default {
    name: `"Header"`,
    components: {
        SvgComponent,
    }
}
</script>

<style scoped>

</style>