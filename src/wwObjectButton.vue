<template>
    <p class="transition_rouge">
        <a href target="_blank">My button</a>
    </p>
</template>

<script>
export default {
    name: "__COMPONENT_NAME__",
    props: {
        wwObjectCtrl: Object,
        wwAttrs: {
            type: Object,
            default: {},
        },
    },
    data() {
        return {
        };
    },
    computed: {
        wwObject() {
            return this.wwObjectCtrl.get();
        },
    },
    methods: {
        init() { },
    },
    mounted() {
        this.init();

        this.$emit("ww-loaded", this);
    },
    beforeDestroy() { },
};
</script>

<style scoped>
</style>
