<template>
  <div class="body">
    <Preloader/>
    <Header />
    <main>
      <div class="main__container container">
        <Nuxt />
      </div>
    </main>
    <Footer />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Footer from "@/components/Footer.vue";
import Preloader from "@/components/Preloader.vue";
export default{
  components: {
    Header,
    Footer,
    Preloader
  }
}
</script>