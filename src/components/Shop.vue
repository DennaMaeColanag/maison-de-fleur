<script>
export default {
    props: ['newAddProduct'],
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
            cards2: [
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
                {
                    id: 4,
                    img: "https://i.pinimg.com/736x/33/c2/3c/33c23c6570d251abd1d20c1be199b32e.jpg",
                    detail: "Sunset Garden Reverie ",
                    price: 699
                },
                {
                    id: 5,
                    img: "https://i.pinimg.com/736x/2a/83/f6/2a83f6ef9bbf78a8196f3286499711a8.jpg",
                    detail: "Wooden Bowl Centerpiece",
                    price: 1200
                },
                {
                    id: 6,
                    img: "https://i.pinimg.com/736x/f8/06/47/f80647d87b516f88d08419f54ebcaa71.jpg",
                    detail: "Little Songbird Sunflower Pot",
                    price: 500
                },
                {
                    id: 7,
                    img: "https://i.pinimg.com/1200x/4e/33/0a/4e330a64ee10dd42b2c24ea27c0ec0c0.jpg",
                    detail: "White Lily & Greenery Trough",
                    price: 999
                },
                {
                    id: 8,
                    img: "https://i.pinimg.com/736x/b3/d2/74/b3d2744bed74927738c95689176dae27.jpg",
                    detail: "Cascading Bridal Bouquet ",
                    price: 1000
                },
                {
                    id: 9,
                    img: "https://i.pinimg.com/1200x/ff/6c/a6/ff6ca658cfd2507351875b590208930a.jpg",
                    detail: "Store Opening Sunshine ",
                    price: 1300
                },
            ],

            detailCard: [
                {
                    id: 1,
                    img: "https://i.pinimg.com/736x/f1/64/d0/f164d079da79c7ee43952515101a1cb3.jpg",
                    details: "Midnight Velvet  Red Roses ",
                    description: "The Midnight Velvet Red Roses arrangement features rich crimson roses, baby's breath, and eucalyptus wrapped in dusty rose paper and tied with a burgundy ribbon for the ultimate romantic gesture.",
                    price: 900,
                    tags: "Eco-Friendly Wrap • Fragrant Blooms • Statement Bouquet • Burlap & Ribbon • Large Bouquet",


                },
                {
                    id: 2,
                    img: "https://i.pinimg.com/736x/fd/2b/5e/fd2b5e1680cb8f65e4ba6860bf04c144.jpg",
                    details: "Vibrant Garden Symphony ",
                    description: "A radiant burst of sunshine in a bouquet! Featuring a magnificent central sunflower framed by vivid orange gerberas, colorful roses, and lush garden blooms, this rustic arrangement brings instant warmth, joy, and positivity to any space.",
                    price: 600,
                    tags: "Vibrant Sunflower & Gerberas • Rustic Burlap Hessian Wrap • Bright & Cheerful Palette "

                },
                {
                    id: 3,
                    img: "https://i.pinimg.com/736x/1a/94/f8/1a94f80afda1fe90c800d780f19525ad.jpg",
                    details: "Golden Sunshine ",
                    description: "A delightful and minimalist arrangement featuring two radiant sunflowers framed by delicate white baby’s breath. Wrapped in rustic brown Kraft paper and tied with a soft cream satin bow, this cheerful bouquet is a sweet, simple way to send sunshine, love, or congratulations.",
                    price: 350,
                    tags: "Twin Sunflowers • Kraft Paper Wrap • Cream Satin Ribbon • Baby’s Breath Accents • Minimalist Rustic Bouquet ",


                },
                {
                    id: 4,
                    img: "https://i.pinimg.com/736x/33/c2/3c/33c23c6570d251abd1d20c1be199b32e.jpg",
                    details: "Sunset Garden Reverie ",
                    description: "A vibrant and grand arrangement featuring dramatic pink Stargazer lilies, a sunny golden sunflower, and a colorful mix of daisies and roses. ",
                    price: 699,
                    tags: "Stargazer Pink Lilies • Bright Sunflower • Rustic Hessian Burlap Wrap • Gingham Plaid & Satin Ribbon",


                },
                {
                    id: 5,
                    img: "https://i.pinimg.com/736x/2a/83/f6/2a83f6ef9bbf78a8196f3286499711a8.jpg",
                    details: "Wooden Bowl Centerpiece ",
                    description: "A vibrant floral centerpiece artfully arranged in a rustic wooden bark bowl. Featuring bright gerbera daisies, soft pink roses, and tall snapdragons, this charming arrangement adds a lively, natural touch to any dining or event table.",
                    price: 1200,
                    tags: "Colorful Table Centerpiece • Wooden Bark Bowl • Vibrant Gerbera Daisies • Pastel Pink Roses ",


                },
                {
                    id: 6,
                    img: "https://i.pinimg.com/736x/f8/06/47/f80647d87b516f88d08419f54ebcaa71.jpg",
                    details: "Little Songbird Sunflower Pot ",
                    description: "A cheerful tabletop arrangement featuring three vibrant sunflowers, lush greenery, and a cute decorative bird accent. Wrapped in a rustic burlap base tied with a raffia bow .",
                    price: 500,
                    tags: "Trio Sunflowers • Burlap Pot Wrap • Raffia Bow Tie • Decorative Bird Pick ",


                },
                {
                    id: 7,
                    img: "https://i.pinimg.com/1200x/4e/33/0a/4e330a64ee10dd42b2c24ea27c0ec0c0.jpg",
                    details: "White Lily & Greenery Trough ",
                    description: "An elegant, Zen-inspired arrangement featuring pristine white lilies, hydrangeas, and arched greenery set in a sleek low white ceramic dish.",
                    price: 999,
                    tags: "Elegant White Lilies • Modern Low Rectangular Vessel • Ikebana-Inspired Design ",


                },
                {
                    id: 8,
                    img: "https://i.pinimg.com/736x/b3/d2/74/b3d2744bed74927738c95689176dae27.jpg",
                    details: "Cascading Bridal Bouquet",
                    description: "An elegant cascading bridal bouquet featuring white roses, calla lilies, and baby's breath, beautifully wrapped in vintage lace with memorial photo charms for a timeless and classic bridal look.",
                    price: 1000,
                    tags: "Elegant White Roses & Calla Lilies • Cascading Bridal Bouquet • Vintage Lace & Memorial Charm Details ",


                },
                {
                    id: 9,
                    img: "https://i.pinimg.com/1200x/ff/6c/a6/ff6ca658cfd2507351875b590208930a.jpg",
                    details: "Store Opening Sunshine ",
                    description: "A colorful grand opening floral stand featuring bright sunflowers, a blue hydrangea, pink gerberas, and roses, arranged on a rustic wooden tripod stand for a festive celebration.",
                    price: 1300,
                    tags: "Vibrant Grand Opening Floral Stand • Sunflowers, Hydrangeas & Pink Roses ",


                },
            ],
            // AddProducts: [
            //     {
            //         id: 1,
            //         img:"",
            //         Name:"",
            //         Price:600,
            //     }
            // ],
            newProduct: [],
            flowerssection: true,
            shopmodal: false,
            detailModal: false,
            addProduct: false
        }
    },
    mounted(){
        this.newProduct.push(...this.newAddProduct)
        console.log(this.newProduct)
    },
    methods: {
        viewAll(index) {
            this.shopmodal = true;
            this.flowerssection = false;
            this.$emit('send-cards', this.cards2[index]);
        },

        detailBtn(index, i) {
            this.$emit('to-detail', this.detailCard[index], i);
            // this.detailModal = true;
        },

        toOrders(or) {
            this.$emit('to-order', or);

        },

        showAddModal() {
            this.addProduct = true;
        },

        cancelAdd() {
            this.addProduct = false;
        },

        newDetailBtn(index, i){
            this.$emit('tonew-detail', this.newProduct[index], i)
        }

    }
}
</script>

<template>
    <div class="bg-[#FAE6ED] w-full h-fit pb-10">

        <div v-if="flowerssection">
            <div class="flex justify-between items-center px-20 pt-35">
                <p class="text-gray-600 text-3xl">Shop Our Collections</p>
                <div class="flex gap-10">
                    <button @click="viewAll(index)"
                        class="bg-[#ee0f3cbd] px-8 py-2 rounded-full shadow-lg shadow-black/50 text-white text-lg flex items-center">VIEW
                        ALL<svg class="w-8 h-7" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 640 640">
                            <path fill="rgb(255, 255, 255)"
                                d="M598.6 342.6C611.1 330.1 611.1 309.8 598.6 297.3L470.6 169.3C458.1 156.8 437.8 156.8 425.3 169.3C412.8 181.8 412.8 202.1 425.3 214.6L498.7 288L64 288C46.3 288 32 302.3 32 320C32 337.7 46.3 352 64 352L498.7 352L425.3 425.4C412.8 437.9 412.8 458.2 425.3 470.7C437.8 483.2 458.1 483.2 470.6 470.7L598.6 342.7z" />
                        </svg></button>
                </div>
            </div>

            <div class="flex justify-center items-center gap-10 py-10 ">
                <div v-for="(card, index) in cards" :key="card.id"
                    class="bg-[#787075cb] w-100 h-100 rounded-3xl shadow-lg shadow-black/50">
                    <div class="">
                        <img class="w-full h-80 rounded-t-3xl" :src="card.img" alt="">
                        <p class="text-black font-bold text-xl px-3">{{ card.detail }}</p>
                        <div class="flex justify-between items-center px-3">
                            <p class="text-gray-800 font-semibold text-lg"> ₱{{ card.price }}.00</p>
                            <button @click="viewAll(index)" class="rounded-full bg-[#eaea15] p-2">
                                <svg class="w-6 h-6" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 640 640">
                                    <path fill="rgb(255, 255, 255)"
                                        d="M598.6 342.6C611.1 330.1 611.1 309.8 598.6 297.3L470.6 169.3C458.1 156.8 437.8 156.8 425.3 169.3C412.8 181.8 412.8 202.1 425.3 214.6L498.7 288L64 288C46.3 288 32 302.3 32 320C32 337.7 46.3 352 64 352L498.7 352L425.3 425.4C412.8 437.9 412.8 458.2 425.3 470.7C437.8 483.2 458.1 483.2 470.6 470.7L598.6 342.7z" />
                                </svg>
                            </button>
                        </div>
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
        <div v-if="shopmodal" class="">
            <div class="flex justify-between items-center px-20 pt-35">
                <p class="text-gray-600 text-3xl">Our Collections</p>
                <button @click="toOrders('Orders')"
                    class="bg-[#ee0f3cbd] px-8 py-2 rounded-full shadow-lg shadow-black/50 text-white text-lg flex items-center">ORDERS<svg
                        class="w-8 h-7" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 640 640">
                        <path fill="rgb(255, 255, 255)"
                            d="M598.6 342.6C611.1 330.1 611.1 309.8 598.6 297.3L470.6 169.3C458.1 156.8 437.8 156.8 425.3 169.3C412.8 181.8 412.8 202.1 425.3 214.6L498.7 288L64 288C46.3 288 32 302.3 32 320C32 337.7 46.3 352 64 352L498.7 352L425.3 425.4C412.8 437.9 412.8 458.2 425.3 470.7C437.8 483.2 458.1 483.2 470.6 470.7L598.6 342.7z" />
                    </svg></button>
            </div>

            <div class="flex justify-center items-center py-10">
                <div class="grid grid-cols-3 gap-10">
                    <div v-for="(card1, index) in cards2" :key="index.id"
                        class="bg-[#787075cb] w-100 h-100 rounded-3xl shadow-lg shadow-black/50">
                        <div class="">
                            <img class="w-full h-80 rounded-t-3xl" :src="card1.img" alt="">
                            <p class="text-black font-bold text-xl px-3">{{ card1.detail }}</p>
                            <div class="flex justify-between items-center px-3">
                                <p class="text-gray-800 font-semibold text-lg"> ₱{{ card1.price }}.00</p>
                                <button @click="detailBtn(index, true)"
                                    class="rounded-full bg-[#eaea15] px-2 py-1 cursor-pointer">
                                    DETAILS
                                </button>
                            </div>
                        </div>

                    </div>
                </div>
            </div>


            <!-- for adding products -->
            <div class="">
                <div class="flex justify-center items-center py-10">
                    <div class="grid grid-cols-3 gap-10">
                        <div v-for="(addP, index) in newAddProduct" :key="addP.id"
                            class="bg-[#787075cb] w-100 h-100 rounded-3xl shadow-lg shadow-black/50">
                            <div class="relative">
                                <div class="absolute -right-3 -top-5">
                                    <h1 class="bg-red-600 px-8 py-2 rounded-3xl text-white font-bold">New</h1>
                                </div>
                                    <img class="w-full h-80 rounded-t-3xl" :src="addP.img" alt="">
                                <p class="text-black font-bold text-xl px-3">{{ addP.details }}</p>
                                <div class="flex justify-between items-center px-3">
                                    <p class="text-gray-800 font-semibold text-lg"> ₱{{ addP.price }}.00</p>
                                    <button @click="newDetailBtn(index, true)"
                                        class="rounded-full bg-[#eaea15] px-2 py-1 cursor-pointer">
                                        DETAILS
                                    </button>
                                </div>
                            </div>

                        </div>
                    </div>
                </div>

            </div>
        </div>

        
    </div>
</template>