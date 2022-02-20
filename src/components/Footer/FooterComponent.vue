<template>
    <footer class="footer footer_bg">
        <div class="container">
            <div class="row">
                <FooterIcons/>
                <FooterNavigation :footerMenu="footerMenu"/>
                <FooterClient :footerClientMenu="footerClientMenu"/>
                <FooterContacts/>
            </div>
        </div>
    </footer>
</template>

<script>
import {menuList, menuClientList} from '../../constants/menuLinks';
import FooterIcons from './FooterIcons';
import FooterNavigation from './FooterNavigation';
import FooterClient from './FooterClient';
import FooterContacts from './FooterContacts';
export default {
    data() {
        return {
            footerMenu: menuList,
            footerClientMenu: menuClientList,
        }
    },
    components: {
        FooterIcons,
        FooterNavigation,
        FooterClient,
        FooterContacts,
    }
}
</script>