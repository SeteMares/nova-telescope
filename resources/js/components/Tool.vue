<script>
export default {
    data: function () {
        return {
            path: "telescope",
        };
    },

    created() {
    },

    computed: {
        telescopePath: function () {
            return ("/" + this.path)
                .replace("\/\/", "\/");
        },
    },

    methods: {

    },
}
</script>

<template>
    <iframe
        :src="telescopePath"
        class="w-full"
        frameborder="0"
        scrolling="auto"
    />
</template>

<style scoped lang="scss">
    iframe {
        margin-top: -50px;
        height: 100vh;
    }
</style>
