<script>
export default {
    props: ['toViewOrder', 'totalAll'],
    data() {
        return {

        }
    },
    methods: {


    }
}
</script>

<template>
    <div class="bg-[#FAE6ED] w-full h-fit">
        <div class="pt-30 px-10">
            <p class="text-gray-700 font-arial font-bold text-2xl py-1">ORDERS</p>
            <div class="bg-[#D9D9D9] shadow-2xl w-30 h-30 rounded-xl ml-10">
                <p class="text-center text-gray-700 font-semibold py-2">Total Items:</p>
                <p class="text-gray-700 font-arial font-bold text-5xl text-center">{{ toViewOrder.length }}</p>
            </div>
        </div>
        <div class="flex justify-center items-center py-10">
            <div class="grid grid-cols-3 gap-10">
                <div v-for="(cart, index) in toViewOrder" :key="index.id"
                    class="bg-[#787075cb] w-100 h-100 rounded-3xl shadow-lg shadow-black/50">
                    <div class="">
                        <img class="w-full h-80 rounded-t-3xl" :src="cart.img" alt="">
                        <p class="text-black font-bold text-xl px-3">{{ cart.details }}</p>
                        <div class="flex justify-between items-center px-3">
                            <p class="text-gray-800 font-semibold text-lg"> ₱{{ cart.price }}.00</p>
                        </div>
                    </div>

                </div>
            </div>
        </div>
        <div class="border-b border-gray-600 w-full flex items-center"></div>
        <div class="flex justify-between items-center py-5 px-10">
            <p class="text-gray-700 font-arial font-bold text-2xl">TOTAL:</p>
            <p class="text-gray-700 font-arial font-bold text-2xl">₱{{ totalAll }}</p>
        </div>
    </div>
</template>