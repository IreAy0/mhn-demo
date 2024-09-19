<template>
  <li>
    <NuxtLink
      :to="item.route"
      class="group relative flex items-center gap-3 font-dmSans rounded-sm py-2 px-4 font-medium text-body duration-300 ease-in-out text-base"
      
    >
      <span v-html="item.icon"></span>
      {{ item.label }}
    </NuxtLink>
    </li>
</template>

<script setup>

const props = defineProps(['item', 'index'])
const currentPage = useRoute().name

</script>

<style scoped>


</style>