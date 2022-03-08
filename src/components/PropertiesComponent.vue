<template>
    <div class="properties">
        <div class="container">
            <div class="row">
                <div class="col-md-12 col-sm-12">
                    <h2 class="properties__h2">
                        Featured <b>Properties</b>
                    </h2>
                </div>
                <div class="col-md-12 col-sm-12">
                    <div class="properties__subtitle">
                        Quisque diam lorem interdum vitaapibus vitae pede. Donec eget tellus non erat lacinia fertum. Donec in velit vel ipsum auctovinar.
                    </div>
                </div>
            </div>
            <div class="row">
                <div class="col-md-4 col-sm-12" v-for="property in propertyData" :key="property.id">
                    <div class="properties__col">
                        <img :src="require(`../assets/images/${property.image}.png`)" :alt="property.desc.sqft" class="properties__img">
                        <h4 class="properties__h4">{{property.title}}</h4>
                        <p class="properties__sub">{{property.subtitle}}</p>
                        <p class="properties__price">${{property.price.toFixed(3)}}</p>
                        <ul class="properties__desc">
                            <li class="properties__item">{{property.desc.sqft}} Sq Ft</li>
                            <li class="properties__item">{{property.desc.rooms}} Bedrooms</li>
                            <li class="properties__item">{{property.desc.bath}} Bathroom</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        <div class="col"><button type="button" class="btn btn-primary properties__more">ALL Properties</button></div>
    </div>
</template>

<script>
export default {
    props: {
        propertyData: {
            type: Array,
            default: () => [],
        }
    }
}
</script>

<style>

</style>