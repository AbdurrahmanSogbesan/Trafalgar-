<template>
            <ul class="list">
                <li class="title">{{ link.title }}</li>
                <li class="subtext" v-for="(link, index) in link.links" :key="index">{{ link }}</li>
            </ul>
</template>

<script>
    export default {
        props: {
            link: Object
        },
    }
</script>

<style lang="scss" scoped>
    .list {
        list-style: none;
        color: #FFF;
        padding-left: 0;
        margin-right: 111px;

        
    @media (max-width:480px) {
        padding-left: 0;
        margin-right: unset;
    }
}
    .title {
        font-weight: bold;
        font-size: 20px;
        line-height: 60px;
    }
    .subtext {
        font-weight: 300;
        font-size: 18px;
        line-height: 38px;
    }
</style>