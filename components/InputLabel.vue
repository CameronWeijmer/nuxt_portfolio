<template>
    <div>
        <label :for="labelFor" class="block text-gray-600 font-medium mb-1">{{ labelText }}<span class="text-[#ff0000]">{{
            star }}</span></label>
        <input :type="inputType" :id="inputId" :name="inputName"
            class="w-full px-3 py-2 border rounded-md focus:outline-none focus:ring-0 focus:border-primary duration-500"
            required :placeholder="inputPlace" />
    </div>
</template>

<script setup>
const probs = defineProps({
    labelFor: String,
    labelText: String,
    star: String,
    inputName: String,
    inputType: String,
    inputId: String,
    inputPlace: String,
})
</script>

<style scoped></style>