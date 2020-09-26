<template>
  <div id="app" class="">
    <div id="nav">
      <Navbar />
    </div>
   <div class="container">
      <router-view/>
   </div>
  </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue'
export default {
    components: {
      Navbar
    }
}
</script>