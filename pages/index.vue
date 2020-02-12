<template>
    <div class="container">
        <ProductZoomerWrapper />
        <nuxt-link to="next">Next!</nuxt-link>
    </div>
</template>

<script>
import ProductZoomerWrapper from "~/components/ProductZoomerWrapper.vue";

export default {
    components: {
        ProductZoomerWrapper
    },
    mounted() {
        location.reload();
    }
};
</script>