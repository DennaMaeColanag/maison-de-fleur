<script>
export default {
    emit:['send-this'],
    data() {
        return {
            newImage: '',
            newDetail: '',
            newDescription: '',
            newPrice: '',
            newTags:''
        }
    },
    methods: {
        cancelAdd(page) {
            this.$emit('gotoHome', page)
        },

        addBtn() {
            this.$emit('send-this', {
                img: this.newImage,
                details: this.newDetail,
                description: this.newDescription,
                price: this.newPrice,
                tags: this.newTags
            })
            alert('Product added successfully!')
        }
    }
}
</script>

<template>
    <div class="bg-blue-200 w-full h-screen flex justify-center items-center pt-20">
        <div class="bg-gray-100 rounded-2xl h-fit shadow-xl pb-10 px-5">
            <p class="text-gray-700 font-bold font-arial text-2xl text-center py-3">New Product</p>

            <div class="px-5">
                <p class="text-gray-700 font-arial text-md pt-3">Product Image URL:</p>
                <input v-model="newImage" class="text-md w-full border border-gray-500 rounded-lg px-5 py-2" type="text"
                    placeholder="Paste image URL here">
            </div>
            <div class="px-5">
                <p class="text-gray-700 font-arial text-md pt-3">Product Name:</p>
                <input v-model="newDetail" class="text-md w-full border border-gray-500 rounded-lg px-5 py-2" type="text"
                    placeholder="Enter product name">
            </div>

            <div class="px-5">
                <p class="text-gray-700 font-arial text-md pt-3">Product Description:</p>
                <input v-model="newDescription" class="text-md w-full border border-gray-500 rounded-lg px-5 py-2" type="text"
                    step="0.01" placeholder="Enter product price">
            </div>
            <div class="px-5">
                <p class="text-gray-700 font-arial text-md pt-3">Product Price:</p>
                <input v-model="newPrice" class="text-md w-full border border-gray-500 rounded-lg px-5 py-2" type="number"
                    step="0.01" placeholder="Enter product price">
            </div>
            <div class="px-5">
                <p class="text-gray-700 font-arial text-md pt-3">Product Tags:</p>
                <input v-model="newTags" class="text-md w-full border border-gray-500 rounded-lg px-5 py-2" type="text"
                    step="0.01" placeholder="Enter product tags">
            </div>


            <div class="flex justify-center items-center gap-5 mt-5">
                <button @click="addBtn"
                    class="bg-blue-500 hover:bg-blue-600 text-white px-5 py-2 rounded-lg w-68 text-center text-lg cursor-pointer transition-colors">
                    Add
                </button>
                <button @click="cancelAdd('Home')"
                    class="bg-red-500 hover:bg-red-600 text-white px-5 py-2 rounded-lg w-68 text-center text-lg cursor-pointer transition-colors">
                    Cancel
                </button>
            </div>
        </div>
    </div>
</template>