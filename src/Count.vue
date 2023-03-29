<script lang="ts">
export default {
    data() {
        return {
            count: 0
        }
    },

    methods: {
        increment() {
            console.log("increment", this.count++);

            // this.count++
        }
    },

    mounted() {
        console.log(`The initial count is ${this.count}`);
    }
}


// import { ref, onMounted } from 'vue';
// const count = ref(0);
// console.log("instance created");
// function increment() {
//     count.value++
// }

</script>

<template>
    <button @click="increment"> Count is : {{ count }}</button>
</template>