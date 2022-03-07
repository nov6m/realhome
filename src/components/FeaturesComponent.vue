<template>
  <div class="feature">
      <div class="container">
        <div class="feature row">
            <div class="col-md-3" v-for="(item) in data" :key="item.id">
                <div class="feature__col feature__col__pad">
                    <img :src="require(`../assets/images/icons/${item.icon}.png`)" class="feature__icon" :alt="item.title"/>
                    <h4 class="feature__title">{{item.title}}</h4>
                    <p class="feature__p">{{item.text}}</p>
                </div>
            </div>
        </div>
      </div>
  </div>
</template>

<script>
export default {
    props: {
        data: {
            type: Array,
            default: () => [],
        }
    },
}
</script>

<style>

</style>template>