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
    <div class="bg-[#FAE6ED] w-full min-h-screen">
        <div class="pt-24 sm:pt-30 px-4 sm:px-10">
            <p class="text-gray-700 font-arial font-bold text-2xl py-1">ORDERS</p>
            <div class="bg-[#D9D9D9] shadow-2xl w-28 h-28 sm:w-30 sm:h-30 rounded-xl ml-4 sm:ml-10 flex flex-col justify-center items-center">
                <p class="text-center text-gray-700 font-semibold py-1 text-sm sm:text-base">Total Items:</p>
                <p class="text-gray-700 font-arial font-bold text-4xl sm:text-5xl text-center">{{ toViewOrder.length }}</p>
            </div>
        </div>
        <div class="flex justify-center items-center py-10 px-4 sm:px-6">
            
            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6 sm:gap-10 w-full max-w-7xl">
                <div v-for="(cart, index) in toViewOrder" :key="index.id"
                    class="bg-[#787075cb] w-full max-w-sm mx-auto sm:max-w-none h-100 rounded-3xl shadow-lg shadow-black/50 overflow-hidden">
                    <div class="">
                        <img class="w-full h-80 object-cover rounded-t-3xl" :src="cart.img" alt="">
                        <p class="text-black font-bold text-xl px-3 mt-2 truncate">{{ cart.details }}</p>
                        <div class="flex justify-between items-center px-3 mt-1">
                            <p class="text-gray-800 font-semibold text-lg"> ₱{{ cart.price }}.00</p>
                        </div>
                    </div>

                </div>
            </div>
        </div>
        <div class="border-b border-gray-600 w-full flex items-center"></div>
        <div class="flex justify-between items-center py-5 px-6 sm:px-10">
            <p class="text-gray-700 font-arial font-bold text-xl sm:text-2xl">TOTAL:</p>
            <p class="text-gray-700 font-arial font-bold text-xl sm:text-2xl">₱{{ totalAll }}</p>
        </div>
    </div>
</template>