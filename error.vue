<template>
  <div class="mt-7 max-w-sm mx-auto text-center card">
    <div class="mt-7 text-7xl font-bold"> {{ error.statusCode}}</div>
    <p class="mt-7">Oooops</p>
    <p class="class mt-7"> {{ error.message }}</p>
    <button @click="handleError" class="my-7 btn my-4 bg-[#12b488] text-white px-3 py-2 rounded-md text-sm text-white">
     GO HOME..
    </button>
  </div>
</template>

<script setup>

const handleError = () => clearError({redirect: "/"})
  defineProps(["error"])
</script>

<style>

</style>