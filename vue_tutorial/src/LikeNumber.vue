<template>
<div>
<p>Like({{ halfNumber }})</p>
<button @click="increment">+1</button>
</div>
    
</template>

<script>
export default {
    props: {
        totalNumber: {
            type: Number,
            default: 10
        },
        testProps: {
            type: String
        }
    },
    computed: {
        halfNumber() {
            return this.number * 2;
        }
    },
    methods: {
        increment() {
            this.number += 1;
        }
    }
};
</script>

<style scoped>
div {
    border: 1px solid red;
}
</style>

