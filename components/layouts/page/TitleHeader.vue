<template>
  <div class="flex gap-1.5 flex-col ">
    <h1 class="text-[36px] text-header5 font-semibold font-Inter">
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