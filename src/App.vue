<template>
  <main-container>
    <template v-slot:header>
    <HeaderComponent/>
    </template>
    <main>
      <router-view/>
    </main>
    <template v-slot:footer>
    <FooterComponent/>
    </template>
  </main-container>
</template>

<script>
import HeaderComponent from '@/components/HeaderComponent.vue'
import FooterComponent from '@/components/Footer/FooterComponent.vue'
import MainContainer from './components/MainContainer.vue'



export default {
  components: {
    MainContainer,
    HeaderComponent,
    FooterComponent,
  },
}
</script>
