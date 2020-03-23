<template>
  <div class="about">
    <Navbar/>

    <Productpage/>

    <Footer />
  </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue'
import Footer from '@/components/Footer.vue'
import Productpage from '@/components/Productpage.vue'


export default {
    name: 'Home',
      components: {
      Productpage,
      Navbar,
      Footer
    }
}
</script>