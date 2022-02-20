<template>
  <div class="wrap d-flex flex-column min-vh-100">
    <HeaderComponent/>
    <main class="flex-fill">
      <router-view/>
    </main>
    <FooterComponent/>
  </div>
</template>

<script>
import HeaderComponent from '@/components/HeaderComponent.vue'
import FooterComponent from '@/components/Footer/FooterComponent.vue'



export default {
  components: {
    HeaderComponent,
    FooterComponent,
  },
}
</script>
