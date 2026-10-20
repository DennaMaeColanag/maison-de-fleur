<script>
import About from './components/About.vue';
import AddProduct from './components/AddProduct.vue';
import Details from './components/Details.vue';
import Flowers from './components/Flowers.vue';
import Footer from './components/Footer.vue';
import Home from './components/Home.vue';
import Navbar from './components/Navbar.vue';
// import Newdetail from './components/Newdetail.vue';
import Orders from './components/Orders.vue';
import Shop from './components/Shop.vue';
export default {
  components: {
    Navbar,
    Home,
    Flowers,
    Shop,
    About,
    Orders,
    Details,
    AddProduct,
    // Newdetail,
    Footer,

  },

  data() {
    return {
      currentPage: 'Home',
      addFlower: [],
      addDetails: [],
      addNewDetails: [],
      myOrder: [],
      newCart: [],
      showModal: false,
      total: 0,
      addText: "",
    }
  },
  methods: {
    section(menu) {
      this.currentPage = menu;
    },
    openFlowerModal(flo) {
      this.addFlower.push(flo);
    },

    openDetailsModal(index, i) {
      this.addDetails.push(index);
      this.showModal = i
    },

    openNewDetailsModal(index, i) {
      // this.addNewDetails.push(index);
      this.addDetails.push(index);
      this.showModal = i
    },
    buycart(index) {
      this.myOrder.push(index);
      this.showModal = false;
      this.addDetails.pop()
      this.total += index.price
    },

    goToShop(page) {
      this.currentPage = page;
    },

    goToOrders(or) {
      this.currentPage = or;
    },

    goToHome(addme) {
      this.currentPage = addme;
    },

    closeModal(i) {
      this.showModal = i
      this.addDetails.pop()
    },

    addProduct(img, details, description, price, tags) {
      this.newCart.push({...img, ...details, ...description, ...price, ...tags});
    },

    navScroll(){
      window.scrollTo({
        top: 0,
        behaviour: 'smooth'
      })
    }


  }
}


</script>

<template>
  <Navbar @click="navScroll" @goTo="section" />
  <Home v-if="currentPage == 'Home'" />
  <Flowers v-if="currentPage == 'Flowers'" @go-to="goToShop" />
  <Shop v-if="currentPage == 'Shop'" @send-cards="openFlowerModal" :newAddProduct="newCart"
    @to-detail="openDetailsModal" @tonew-detail="openNewDetailsModal" @to-order="goToOrders"
    :toViewFlowers="addFlower" />
  <About v-if="currentPage == 'About'" />
  <Orders v-if="currentPage == 'Orders'" :toViewOrder="myOrder" :totalAll=total />
  <Details v-if="showModal === true" @closeModal="closeModal" @clickTobuy="buycart" :toViewDetails="addDetails"
    :newAddProduct="newCart" />
  <AddProduct v-if="currentPage == 'AddProduct'" @send-this="addProduct" />
  <!-- <Newdetail @clickTobuy="buycart" :toViewNewDetails="addNewDetails"/> -->
  <Footer />

</template>
