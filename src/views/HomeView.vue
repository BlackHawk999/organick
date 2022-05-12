<template>
  <div class="home">
    <Navbar />
    <Intro />
    <Offers />
    <About />
    <Products />
    <Reviews />
    <SpecialOffer />
    <Eco />
    <ProductsMenu />
    <News />
    <PreFooter />
    <Footer />
  </div>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
import Intro from "@/components/Intro.vue";
import Offers from "@/components/Offers.vue";
import About from "@/components/About.vue";
import Products from "@/components/products/Products.vue";
import Reviews from "@/components/Reviews.vue";
import SpecialOffer from "@/components/SpecialOffer.vue";
import Eco from "@/components/Eco.vue";
import ProductsMenu from "@/components/products/ProductsMenu.vue";
import News from "@/components/News.vue";
import PreFooter from "@/components/PreFooter.vue";
import Footer from "@/components/Footer.vue";
// @ is an alias to /src

export default {
  components: {
    Navbar,
    Intro,
    Offers,
    About,
    Products,
    Reviews,
    SpecialOffer,
    Eco,
    ProductsMenu,
    News,
    PreFooter,
    Footer,
  },
};
</script>

<style lang="scss" scoped>
.home {
}
</style>
