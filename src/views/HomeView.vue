<template>
  <div class="home">
    <Carusel/>
    <div class="container home_offering">
      <div class="row">
        <div class="col-md-4 home_border">
          <h3 class="home_offeringTitle">We are Offering the Best Estate Deals</h3>
        </div>
        <div class="col-md-8">
          <p>
            Quisque diam lorem interdum vitaapibus ac scelerisque vitae pede. 
            Donec eget tellus non erat lacinia fertum. Donec in velit vel ipsum auctovinar. 
            Proin umcorper urna et felisstibulum iaculis lacinia est. Proin dictum elem entum velit fusce euismod. 
            Aenean commodo ligula eget dolor. Aenean massa. Lorem ipsum dolor sit amet, consec tetuer adipis elit, 
            aliquam eget nibh etlibura. Lorem ipsum dolor sitamet, consetetur sadipscing elitr, sed diam nonumy 
            eirmod tempor invidunt ut labore et.
            </p>
        </div>
      </div>
    </div>
  </div>
</template>


<script>

import Carusel from '../components/CaruselComponent.vue';

export default {
  name: 'HomeView',
  components: {
    Carusel,
  },
}
</script>