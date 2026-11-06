<script>
export default {
    data() {
        return {
            mobileMenuOpen: false
        }
    },
    methods: {
        nav(page) {
            this.$emit('goTo', page);
            this.mobileMenuOpen = false; 
        }
    }
}
</script>

<template>
    <div
        class="bg-white/10 backdrop-blur-md w-full flex justify-between items-center px-4 sm:px-6 md:px-5 py-3 fixed z-999 top-0 left-0">
        <div>
            <img class="w-20 sm:w-25 h-16 sm:h-20 object-contain" src="../assets/flower_logo-removebg-preview.png" alt="">
        </div>

 
        <div class="hidden md:flex items-center gap-6 lg:gap-10">
            <p @click="nav('Home')" class="text-lg font-arial hover:underline hover:text-gray-700 cursor-pointer">Home
            </p>
            <p @click="nav('Flowers')" class="text-lg font-arial hover:underline hover:text-gray-700 cursor-pointer">
                Flowers</p>
            <p @click="nav('Shop')" class="text-lg font-arial hover:underline hover:text-gray-700 cursor-pointer">Shop
            </p>
            <p @click="nav('About')" class="text-lg font-arial hover:underline hover:text-gray-700 cursor-pointer">About
            </p>
            <p @click="nav('Orders')" class="text-lg font-arial hover:underline hover:text-gray-700 cursor-pointer">
                Orders</p>
        </div>

        <div class="flex items-center gap-3 sm:gap-4">
            <svg class="w-6 h-6 sm:w-7 sm:h-7 cursor-pointer hover:opacity-75" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 640 640">
                <path
                    d="M480 272C480 317.9 465.1 360.3 440 394.7L566.6 521.4C579.1 533.9 579.1 554.2 566.6 566.7C554.1 579.2 533.8 579.2 521.3 566.7L394.7 440C360.3 465.1 317.9 480 272 480C157.1 480 64 386.9 64 272C64 157.1 157.1 64 272 64C386.9 64 480 157.1 480 272zM272 416C351.5 416 416 351.5 416 272C416 192.5 351.5 128 272 128C192.5 128 128 192.5 128 272C128 351.5 192.5 416 272 416z" />
            </svg>
            <svg class="w-6 h-6 sm:w-7 sm:h-7 cursor-pointer hover:opacity-75" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 640 640">
                <path
                    d="M320 312C386.3 312 440 258.3 440 192C440 125.7 386.3 72 320 72C253.7 72 200 125.7 200 192C200 258.3 253.7 312 320 312zM290.3 368C191.8 368 112 447.8 112 546.3C112 562.7 125.3 576 141.7 576L498.3 576C514.7 576 528 562.7 528 546.3C528 447.8 448.2 368 349.7 368L290.3 368z" />
            </svg>
            <p @click="nav('AddProduct')" class="text-4xl sm:text-5xl pb-2 sm:pb-3 pl-0 cursor-pointer hover:text-gray-700">+</p>
            
      
            <button @click="mobileMenuOpen = !mobileMenuOpen" class="md:hidden flex flex-col justify-center items-center w-8 h-8 space-y-1.5 focus:outline-none cursor-pointer">
                <span :class="{'rotate-45 translate-y-2': mobileMenuOpen}" class="w-6 h-0.5 bg-gray-800 transition-transform duration-300"></span>
                <span :class="{'opacity-0': mobileMenuOpen}" class="w-6 h-0.5 bg-gray-800 transition-opacity duration-300"></span>
                <span :class="{'-rotate-45 -translate-y-2': mobileMenuOpen}" class="w-6 h-0.5 bg-gray-800 transition-transform duration-300"></span>
            </button>
        </div>
    </div>

   
    <div v-if="mobileMenuOpen" class="md:hidden fixed top-84px left-0 w-full bg-white/90 backdrop-blur-md shadow-lg py-6 px-6 z-998 flex flex-col items-center space-y-4 border-b border-gray-200">
        <p @click="nav('Home')" class="text-lg font-arial hover:text-orange-600 cursor-pointer py-1">Home</p>
        <p @click="nav('Flowers')" class="text-lg font-arial hover:text-orange-600 cursor-pointer py-1">Flowers</p>
        <p @click="nav('Shop')" class="text-lg font-arial hover:text-orange-600 cursor-pointer py-1">Shop</p>
        <p @click="nav('About')" class="text-lg font-arial hover:text-orange-600 cursor-pointer py-1">About</p>
        <p @click="nav('Orders')" class="text-lg font-arial hover:text-orange-600 cursor-pointer py-1">Orders</p>
    </div>
</template>