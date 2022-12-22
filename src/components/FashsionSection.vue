<template>
    <div class="flex my-10 justify-around overflow-visible">
        <div class="relative">
            <div class="z-10 overflow-hidden">
                <img class="z-10" src="../assets/fashion.png" />
            </div>
            <div class="absolute top-[337px] left-[128px] z-[-1] overflow-visible">
                <img class="z-0 overflow-visible" src="../assets/Rectangle.png" />
            </div>
        </div>
        <div class="flex flex-col gap-[60px] items-start justify-center w-[29.5625rem] h-[303px] ">
            <div class="flex flex-col gap-[16px] items-start w-[29.5625rem] h-[184px] grow-0 order-none">
                <div class="bg-[#371D1B] w-[29.5625rem] flex h-[62px] justify-center items-center  rounded-sm">
                    <p class="text-white text-center">Black Friday sales with 20% off on everything </p>
                </div>
                <p class="font-['Playfair_Display'] text-[#371D1B] text-[40px]">Explore our Elegant New Products Today!</p>
            </div>
            <div class="flex justify-center items-center gap-[10px] px-px-[20px 62px] rounded-[1px] border-solid border-2 w-[11.3125rem] h-[3.6875rem] grow-0 order-1">
                <p>Explore</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: `"FashionSection"`
}
</script>