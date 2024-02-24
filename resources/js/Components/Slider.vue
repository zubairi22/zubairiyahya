<template>
    <div class="overflow-x-scroll hide-scrollbar">
        <div class="w-max">
            <div class="flex space-x-4 p-2 ">
                <div v-for="(image) in images">
                    <img :src="image" alt="Image 1" class="w-72 md:w-96 object-cover rounded-lg">
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>

const props = defineProps({
    images: {
        type: Array,
        required: true
    }
});
</script>

<style scoped>
    .hide-scrollbar {
        scrollbar-width: none;
        -ms-overflow-style: none;
    }

    .hide-scrollbar::-webkit-scrollbar {
        display: none;
    }
</style>

