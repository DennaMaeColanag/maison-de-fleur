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
    <div class="bg-[#FAE6ED] w-full h-fit flex justify-center items-center pt-30 pb-10">
        <div class="grid grid-cols-1 gap-5">
            <div class="bg-[#f430fe43] w-300 h-fit rounded-4xl p-8 flex gap-5">
                <div>
                    <img class="w-70 h-70 rounded-xl"
                        src="https://i.pinimg.com/736x/cf/84/c0/cf84c0d76f8996be1ed790350f11ff9b.jpg" alt="">
                </div>
                <div class="relative w-full">
                    <div class="px-18 pt-10">
                        <p class="font-arial text-4xl italic font-semibold">"Endless Devotion" Arrangement</p>
                        <p class="font-arial text-xl pl-5">Express timeless love with this romantic bouquet of deep <br>
                            velvet red roses, soft blush
                            carnations, and delicate <br> baby’s breath. </p>
                    </div>
                    <div class="flex  items-end absolute bottom-0 right-0">
                        <button @click="toShop('Shop')"
                            class="text-white font-arial font-semibold text-md rounded-full px-8 py-2 bg-[#f430fed9]">
                            VIEW FLOWER
                        </button>
                    </div>
                </div>

            </div>
            <div class="bg-[#30b2fe4a] w-300 h-fit rounded-4xl p-8 flex gap-5">
                <div>
                    <img class="w-70 h-70 rounded-xl"
                        src="https://i.pinimg.com/736x/26/50/70/2650708295f9ffc442cfa34d8d42fdf8.jpg" alt="">
                </div>
                <div class="relative w-full">
                    <div class="px-18 pt-10">
                        <p class="font-arial text-4xl italic font-semibold">"Pastel Dream" Tulip Arrangement</p>
                        <p class="font-arial text-xl pl-5">Delicate and timeless, this charming bouquet features soft
                            <br>
                            pink and crisp white tulips intertwined with airy baby’s <br> breath.
                        </p>
                    </div>
                    <div class="flex  items-end absolute bottom-0 right-0">
                        <button @click="toShop('Shop')"
                            class="text-white font-arial font-semibold text-md rounded-full px-8 py-2 bg-[#30b2fed0]">
                            VIEW FLOWER
                        </button>
                    </div>
                </div>

            </div>
            <div class="bg-[#feac3058] w-300 h-fit rounded-4xl p-8 flex gap-5">
                <div>
                    <img class="w-70 h-70 rounded-xl"
                        src="https://i.pinimg.com/736x/3d/d6/6e/3dd66e79fa5fad8e88438c010c5fb93e.jpg" alt="">
                </div>
                <div class="relative w-full">
                    <div class="px-18 pt-10">
                        <p class="font-arial text-4xl italic font-semibold">"Ivory Haven" Oriental Lily Arrangement</p>
                        <p class="font-arial text-xl pl-5">Timeless and serene, this stunning bouquet features grand
                            white lilies <br> in full bloom alongside fresh green buds, delicate baby’s breath, <br> and
                            eucalyptus. </p>
                    </div>
                    <div class="flex  items-end absolute bottom-0 right-0">
                        <button @click="toShop('Shop')"
                            class="text-white font-arial font-semibold text-md rounded-full px-8 py-2 bg-[#feac30e1]">
                            VIEW FLOWER
                        </button>
                    </div>
                </div>

            </div>
            <div class="bg-[#30fe8648] w-300 h-fit rounded-4xl p-8 flex gap-5">
                <div>
                    <img class="w-70 h-70 rounded-xl"
                        src="https://i.pinimg.com/736x/60/15/a3/6015a3c6cbbe0eaa4f1e10298ccb5a76.jpg" alt="">
                </div>
                <div class="relative w-full">
                    <div class="px-18 pt-10">
                        <p class="font-arial text-4xl italic font-semibold">"Blush Opulence" XL Rose Arrangement</p>
                        <p class="font-arial text-xl pl-5">Make an unforgettable declaration of grand romance with this
                            <br>
                            magnificent, oversized bouquet featuring dozens of premium soft-pink <br> and vibrant
                            hot-pink
                            roses. </p>
                    </div>
                    <div class="flex  items-end absolute bottom-0 right-0">
                        <button @click="toShop('Shop')"
                            class="text-white font-arial font-semibold text-md rounded-full px-8 py-2 bg-[#30fe86e9]">
                            VIEW FLOWER
                        </button>
                    </div>
                </div>

            </div>
            <div class="bg-[#d8fe3056] w-300 h-fit rounded-4xl p-8 flex gap-5">
                <div>
                    <img class="w-70 h-70 rounded-xl"
                        src="https://i.pinimg.com/736x/b3/d2/74/b3d2744bed74927738c95689176dae27.jpg" alt="">
                </div>
                <div class="relative w-full">
                    <div class="px-18 pt-10">
                        <p class="font-arial text-4xl italic font-semibold">"Royal Cascade" Bridal Arrangement</p>
                        <p class="font-arial text-xl pl-5">A breathtaking bridal masterpiece, this cascading bouquet <br>
                            combines pristine white roses and sleek calla lilies enveloped in <br> delicate baby’s breath and
                            lush greens. </p>
                    </div>
                    <div class="flex  items-end absolute bottom-0 right-0">
                        <button @click="toShop('Shop')"
                            class="text-white font-arial font-semibold text-md rounded-full px-8 py-2 bg-[#d8fe30ea]">
                            VIEW FLOWER
                        </button>
                    </div>
                </div>

            </div>
        </div>
    </div>
</template>