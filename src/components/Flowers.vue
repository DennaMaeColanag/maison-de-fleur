<script>
export default {
    data() {
        return {

        }
    },
    methods: {
        toShop(page){
            this.$emit('go-to', page)
        }
    }
}
</script>

<template>
    <div class="bg-[#FAE6ED] w-full min-h-screen flex justify-center items-center py-16 sm:py-20 md:pt-30 md:pb-10 px-4 sm:px-6">
        <div class="grid grid-cols-1 gap-6 md:gap-5 w-full max-w-5xl">
            
            <div class="bg-[#f430fe43] w-full h-fit rounded-3xl md:rounded-4xl p-4 sm:p-6 md:p-8 flex flex-col md:flex-row items-center md:items-start gap-5">
                <div class="shrink-0">
                    <img class="w-full sm:w-64 md:w-70 h-64 md:h-70 object-cover rounded-xl"
                        src="https://i.pinimg.com/736x/cf/84/c0/cf84c0d76f8996be1ed790350f11ff9b.jpg" alt="">
                </div>
                <div class="relative w-full flex flex-col justify-between h-full min-h-220px md:min-h-280px">
                    <div class="px-2 sm:px-4 md:px-18 pt-2 md:pt-10">
                        <p class="font-arial text-2xl sm:text-3xl md:text-4xl italic font-semibold">"Endless Devotion" Arrangement</p>
                        <p class="font-arial text-base sm:text-lg md:text-xl md:pl-5 mt-2">Express timeless love with this romantic bouquet of deep velvet red roses, soft blush carnations, and delicate baby’s breath.</p>
                    </div>
                    <div class="flex items-end justify-end mt-4 md:absolute md:bottom-0 md:right-0">
                        <button @click="toShop('Shop')"
                            class="text-white font-arial font-semibold text-sm md:text-md rounded-full px-6 md:px-8 py-2 bg-[#f430fed9] cursor-pointer hover:opacity-90 transition-opacity">
                            VIEW FLOWER
                        </button>
                    </div>
                </div>
            </div>

         
            <div class="bg-[#30b2fe4a] w-full h-fit rounded-3xl md:rounded-4xl p-4 sm:p-6 md:p-8 flex flex-col md:flex-row items-center md:items-start gap-5">
                <div class="shrink-0">
                    <img class="w-full sm:w-64 md:w-70 h-64 md:h-70 object-cover rounded-xl"
                        src="https://i.pinimg.com/736x/26/50/70/2650708295f9ffc442cfa34d8d42fdf8.jpg" alt="">
                </div>
                <div class="relative w-full flex flex-col justify-between h-full min-h-220px md:min-h-280px">
                    <div class="px-2 sm:px-4 md:px-18 pt-2 md:pt-10">
                        <p class="font-arial text-2xl sm:text-3xl md:text-4xl italic font-semibold">"Pastel Dream" Tulip Arrangement</p>
                        <p class="font-arial text-base sm:text-lg md:text-xl md:pl-5 mt-2">Delicate and timeless, this charming bouquet features soft pink and crisp white tulips intertwined with airy baby’s breath.</p>
                    </div>
                    <div class="flex items-end justify-end mt-4 md:absolute md:bottom-0 md:right-0">
                        <button @click="toShop('Shop')"
                            class="text-white font-arial font-semibold text-sm md:text-md rounded-full px-6 md:px-8 py-2 bg-[#30b2fed0] cursor-pointer hover:opacity-90 transition-opacity">
                            VIEW FLOWER
                        </button>
                    </div>
                </div>
            </div>

      
            <div class="bg-[#feac3058] w-full h-fit rounded-3xl md:rounded-4xl p-4 sm:p-6 md:p-8 flex flex-col md:flex-row items-center md:items-start gap-5">
                <div class="shrink-0">
                    <img class="w-full sm:w-64 md:w-70 h-64 md:h-70 object-cover rounded-xl"
                        src="https://i.pinimg.com/736x/3d/d6/6e/3dd66e79fa5fad8e88438c010c5fb93e.jpg" alt="">
                </div>
                <div class="relative w-full flex flex-col justify-between h-full min-h-220px md:min-h-280px">
                    <div class="px-2 sm:px-4 md:px-18 pt-2 md:pt-10">
                        <p class="font-arial text-2xl sm:text-3xl md:text-4xl italic font-semibold">"Ivory Haven" Oriental Lily Arrangement</p>
                        <p class="font-arial text-base sm:text-lg md:text-xl md:pl-5 mt-2">Timeless and serene, this stunning bouquet features grand white lilies in full bloom alongside fresh green buds, delicate baby’s breath, and eucalyptus.</p>
                    </div>
                    <div class="flex items-end justify-end mt-4 md:absolute md:bottom-0 md:right-0">
                        <button @click="toShop('Shop')"
                            class="text-white font-arial font-semibold text-sm md:text-md rounded-full px-6 md:px-8 py-2 bg-[#feac30e1] cursor-pointer hover:opacity-90 transition-opacity">
                            VIEW FLOWER
                        </button>
                    </div>
                </div>
            </div>

          
            <div class="bg-[#30fe8648] w-full h-fit rounded-3xl md:rounded-4xl p-4 sm:p-6 md:p-8 flex flex-col md:flex-row items-center md:items-start gap-5">
                <div class="shrink-0">
                    <img class="w-full sm:w-64 md:w-70 h-64 md:h-70 object-cover rounded-xl"
                        src="https://i.pinimg.com/736x/60/15/a3/6015a3c6cbbe0eaa4f1e10298ccb5a76.jpg" alt="">
                </div>
                <div class="relative w-full flex flex-col justify-between h-full min-h-220px md:min-h-280px">
                    <div class="px-2 sm:px-4 md:px-18 pt-2 md:pt-10">
                        <p class="font-arial text-2xl sm:text-3xl md:text-4xl italic font-semibold">"Blush Opulence" XL Rose Arrangement</p>
                        <p class="font-arial text-base sm:text-lg md:text-xl md:pl-5 mt-2">Make an unforgettable declaration of grand romance with this magnificent, oversized bouquet featuring dozens of premium soft-pink and vibrant hot-pink roses.</p>
                    </div>
                    <div class="flex items-end justify-end mt-4 md:absolute md:bottom-0 md:right-0">
                        <button @click="toShop('Shop')"
                            class="text-white font-arial font-semibold text-sm md:text-md rounded-full px-6 md:px-8 py-2 bg-[#30fe86e9] cursor-pointer hover:opacity-90 transition-opacity">
                            VIEW FLOWER
                        </button>
                    </div>
                </div>
            </div>

            <div class="bg-[#d8fe3056] w-full h-fit rounded-3xl md:rounded-4xl p-4 sm:p-6 md:p-8 flex flex-col md:flex-row items-center md:items-start gap-5">
                <div class="shrink-0">
                    <img class="w-full sm:w-64 md:w-70 h-64 md:h-70 object-cover rounded-xl"
                        src="https://i.pinimg.com/736x/b3/d2/74/b3d2744bed74927738c95689176dae27.jpg" alt="">
                </div>
                <div class="relative w-full flex flex-col justify-between h-full min-h-220px md:min-h-280px">
                    <div class="px-2 sm:px-4 md:px-18 pt-2 md:pt-10">
                        <p class="font-arial text-2xl sm:text-3xl md:text-4xl italic font-semibold">"Royal Cascade" Bridal Arrangement</p>
                        <p class="font-arial text-base sm:text-lg md:text-xl md:pl-5 mt-2">A breathtaking bridal masterpiece, this cascading bouquet combines pristine white roses and sleek calla lilies enveloped in delicate baby’s breath and lush greens.</p>
                    </div>
                    <div class="flex items-end justify-end mt-4 md:absolute md:bottom-0 md:right-0">
                        <button @click="toShop('Shop')"
                            class="text-white font-arial font-semibold text-sm md:text-md rounded-full px-6 md:px-8 py-2 bg-[#d8fe30ea] cursor-pointer hover:opacity-90 transition-opacity">
                            VIEW FLOWER
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>