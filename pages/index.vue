<template>
    <div class="container">
        <ProductZoomerWrapper :key="componentKey" />
        <nuxt-link to="next">Next!</nuxt-link>
    </div>
</template>

<script>
import ProductZoomerWrapper from "~/components/ProductZoomerWrapper.vue";

export default {
    components: {
        ProductZoomerWrapper
    },
    data() {
        return {
            componentKey: 0
        };
    },
    methods: {
        forceRerender() {
            this.componentKey += Math.floor(Math.random() * Math.floor(9999));
        }
    },
    mounted() {
        this.forceRerender();
    }
};
</script>