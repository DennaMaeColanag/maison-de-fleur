<script>
export default {
    data() {
        return {
            cards: [
                {
                    id: 1,
                    img: "https://i.pinimg.com/736x/f1/64/d0/f164d079da79c7ee43952515101a1cb3.jpg",
                    detail: "Midnight Velvet  Red Roses ",
                    price: 900
                },
                {
                    id: 2,
                    img: "https://i.pinimg.com/736x/fd/2b/5e/fd2b5e1680cb8f65e4ba6860bf04c144.jpg",
                    detail: "Vibrant Garden Symphony ",
                    price: 600
                },
                {
                    id: 3,
                    img: "https://i.pinimg.com/736x/1a/94/f8/1a94f80afda1fe90c800d780f19525ad.jpg",
                    detail: "Golden Sunshine ",
                    price: 350
                },
            ],
            flowerssection: true,
            shopmodal: true,
        }
    },
    methods: {

    }
}
</script>

<template>
    <div class="bg-[#FAE6ED] w-full h-fit pb-10">
        <div class="flex justify-between items-center px-20 pt-35">
            <p class="text-gray-600 text-3xl">Shop Our Collections</p>
            <button
                class="bg-[#ee0f3cbd] px-8 py-2 rounded-full shadow-lg shadow-black/50 text-white text-lg flex items-center">VIEW
                ALL<svg class="w-8 h-7" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 640 640">
                    <path fill="rgb(255, 255, 255)"
                        d="M598.6 342.6C611.1 330.1 611.1 309.8 598.6 297.3L470.6 169.3C458.1 156.8 437.8 156.8 425.3 169.3C412.8 181.8 412.8 202.1 425.3 214.6L498.7 288L64 288C46.3 288 32 302.3 32 320C32 337.7 46.3 352 64 352L498.7 352L425.3 425.4C412.8 437.9 412.8 458.2 425.3 470.7C437.8 483.2 458.1 483.2 470.6 470.7L598.6 342.7z" />
                </svg></button>
        </div>
        <div v-if="flowerssection" class="flex justify-center items-center gap-10 py-10 ">
            <div v-for="(card, index) in cards" :key="card.id"
                class="bg-[#787075cb] w-100 h-100 rounded-3xl shadow-lg shadow-black/50">
                <div class="">
                    <img class="w-full h-80 rounded-t-3xl" :src="card.img" alt="">
                    <p class="text-black font-bold text-xl px-3">{{ card.detail }}</p>
                    <p class="text-gray-800 font-semibold text-lg px-3"> ₱{{ card.price }}.00</p>
                </div>

            </div>

        </div>
        <div class="flex justify-center">
            <div class="bg-[#fe305666] w-350 h-80 flex items-center ">
                <div class="w-100 px-5 space-y-2">
                    <p class="text-2xl font-arial text-gray-500 font-bold">FLOWERS THAT TELL BEAUTIFUL STORIES</p>
                    <p class=" text-gray-500 font-arial text-md ">We source the finest blooms and design
                        with heart to bring beauty, joy, and meaning to every moment.</p>
                    <button
                        class="bg-[#ee0f3cbd] px-8 py-2  rounded-full shadow-lg shadow-black/50 text-white text-lg ml-50 mt-5">OUR
                        STORY
                    </button>
                </div>
                <div>
                    <img class="w-250 h-80 object-fit rounded-l-3xl"
                        src="https://i.pinimg.com/1200x/4f/ea/51/4fea51b444caa855e8c6a2e705ffaaf5.jpg" alt="">
                </div>

            </div>
        </div>

    </div>
</template>