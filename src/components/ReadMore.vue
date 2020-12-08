<template>
    <div class="read-more">
        <div class="text">Read More</div>
        <DownloadIcon class="rotate"/>
    </div>
</template>

<script>
    import DownloadIcon from "./DownloadIcon.vue"

    export default {
        components: {
            DownloadIcon,
        },
    }
</script>

<style lang="scss" scoped>
    .read-more {
        display: flex;
        flex-direction: row;
        align-items: center;
    }
    .text {
        font-weight: 600;
        font-size: 17px;
        line-height: 28px;
        color: #4089ED;
        margin-right: 12px;
    }
    .rotate {
        transform: rotate(-90deg);
    }
</style>