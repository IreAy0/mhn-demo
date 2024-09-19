<template>
  <div class="flex gap-2 flex-col mt-4">
    <h1 class="text-[28px] text-header5 font-medium font-dmSans">
    {{title}}
    </h1>
    <p class="text-header text-base font-normal">
      {{subTitle}}
    </p>
  </div>
</template>

<script setup>
defineProps({
  title: {
    type: String,
    required: true
  },
  subTitle:{
    type: String
  }
})
</script>

<style lang="scss" scoped>

</style>