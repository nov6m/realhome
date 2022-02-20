<template>
    <div class="col"> 
        <h3 class="footer_title">For clients</h3>
        <ul class="footer_list footer_list_capitalize">
            <li v-for="(menu, index) in footerClientMenu" :key="index">
                <router-link :to="menu.path" class="footer_link">{{menu.name}}</router-link>
            </li>
        </ul>
    </div>
</template>


<script>
export default {
    props: {
        footerClientMenu: {
            type: Array,
            required: true,
        },
    },
}
</script>