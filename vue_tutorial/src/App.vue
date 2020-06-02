<template>
<div>
<LikeHeader></LikeHeader>
<h2>App.vue {{ number }}</h2>
<LikeNumber number="6"></LikeNumber>
</div>

</template>

<script>
import LikeHeader from "./LikeHeader.vue"
export default {
    data() {
        return {
            number: 10
        };
    },
    components: {
        LikeHeader
    }
}
</script>

<style>

</style>
