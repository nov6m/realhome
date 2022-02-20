<template>
    <div class="col">
        <h3 class="footer_title">Contact us</h3>
        <ul class="footer_list footer_list_capitalize">
            <li>
                <p>240 Central Park, London OR 10019</p>
            </li>
            <li class="footer_contacts">
                <p>Freephone: +1 800 559 6580</p>
                <p>elephone: +1 959 603 6035</p>
                <p>FAX: +1 800 559 6580</p>
            </li>
            <li>
                <p><a href="mailto:info@realhome.com" target="blank" class="footer_link footer_link_red footer_link_underline"><p>info@realhome.com</p></a></p>
            </li>
        </ul>
    </div>
</template>


<script>
export default {
    props: {
        footerContacts: {
            type: Array,
            required: true,
        }
    }
}
</script>