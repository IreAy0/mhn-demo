<script lang="ts" setup>
import Breadcrumb from "~/components/Breadcrumb.vue"
definePageMeta({ layout: 'page' })
useHead({ titleTemplate: '', title: 'Dashboard' })
</script>

<template>
  <div>
    <Breadcrumb :breadcrumbs="[
      { text: 'Overview' },
    ]"></Breadcrumb>
    <div>
      <LayoutPageTitleHeader :title="'Overview'" :sub-title="'Manage your account'" />
    </div>

    <div class="mt-4">
      <h2 class="text-header5 text-2xl font-medium">Store Management</h2>
      <div class="grid grid-cols-3 gap-8 mt-4">
        <LayoutPageCard>
          <div class="flex items-center">
            <div class="bg-[#FF965D] bg-opacity-10 h-10 w-[49px] flex items-center justify-center rounded-full p-2 mr-3">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <g clip-path="url(#clip0_8673_420697)">
                <path d="M19 3.00049H12.472C12.3173 3.00151 12.1645 2.96731 12.025 2.90049L8.869 1.31649C8.45239 1.10903 7.9934 1.00087 7.528 1.00049L5 1.00049C3.67441 1.00208 2.40356 1.52937 1.46622 2.46671C0.528882 3.40405 0.00158786 4.67489 0 6.00049L0 18.0005C0.00158786 19.3261 0.528882 20.5969 1.46622 21.5343C2.40356 22.4716 3.67441 22.9989 5 23.0005H19C20.3256 22.9989 21.5964 22.4716 22.5338 21.5343C23.4711 20.5969 23.9984 19.3261 24 18.0005V8.00049C23.9984 6.67489 23.4711 5.40405 22.5338 4.46671C21.5964 3.52937 20.3256 3.00208 19 3.00049ZM5 3.00049L7.528 3.00049C7.68266 2.99947 7.83552 3.03366 7.975 3.10049L11.131 4.67949C11.5472 4.88867 12.0062 4.99855 12.472 5.00049L19 5.00049C19.598 5.00146 20.1821 5.18116 20.6773 5.5165C21.1725 5.85184 21.5561 6.32753 21.779 6.88249L2 6.99449V6.00049C2 5.20484 2.31607 4.44178 2.87868 3.87917C3.44129 3.31656 4.20435 3.00049 5 3.00049ZM19 21.0005H5C4.20435 21.0005 3.44129 20.6844 2.87868 20.1218C2.31607 19.5592 2 18.7961 2 18.0005L2 8.99449L22 8.88149V18.0005C22 18.7961 21.6839 19.5592 21.1213 20.1218C20.5587 20.6844 19.7956 21.0005 19 21.0005Z" fill="#DC6803"/>
                </g>
                <defs>
                <clipPath id="clip0_8673_420697">
                <rect width="24" height="24" fill="white"/>
                </clipPath>
                </defs>
              </svg>
            </div>
            <div>
              <h3 class="text-body font-normal text-base">Prescriptions</h3>
              <p class="text-[#3F434A] font-medium text-base">0</p>
            </div>
            </div>
        </LayoutPageCard>
        <LayoutPageCard >
          <div class="flex items-center">
            <div class="bg-[#A6F4C5] bg-opacity-10 h-10 w-[49px] flex items-center justify-center rounded-full p-2 mr-3">
              <svg width="25" height="20" viewBox="0 0 25 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path fill-rule="evenodd" clip-rule="evenodd" d="M18.2276 7.16984C17.8501 7.50881 17.2081 7.53339 16.7935 7.22474L13.8066 5.00105L13.8066 17.1699C13.8066 17.6284 13.3521 18 12.7914 18C12.2308 18 11.7762 17.6284 11.7762 17.1699L11.7762 5.00105L8.78941 7.22474C8.37484 7.53339 7.73275 7.50881 7.35527 7.16984C6.97779 6.83087 7.00785 6.30588 7.42242 5.99723L12.7914 2L18.1605 5.99723C18.575 6.30588 18.6051 6.83087 18.2276 7.16984Z" fill="#12B76A"/>
                </svg>
                
            </div>
            <div>
              <h3 class="text-body font-normal text-base">Active</h3>
              <p class="text-[#3F434A] font-medium text-base">0</p>
            </div>
            </div>
        </LayoutPageCard>
        <LayoutPageCard >
          <div class="flex items-center">
            <div class="bg-[#304FFD] bg-opacity-10 h-10 w-[49px] flex items-center justify-center rounded-full p-2 mr-3">
              <svg width="26" height="20" viewBox="0 0 26 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path fill-rule="evenodd" clip-rule="evenodd" d="M7.08878 7.16984C7.46626 7.50881 8.10835 7.53339 8.52292 7.22474L11.5098 5.00105V17.1699C11.5098 17.6284 11.9643 18 12.525 18C13.0856 18 13.5402 17.6284 13.5402 17.1699V5.00105L16.527 7.22474C16.9416 7.53339 17.5837 7.50881 17.9611 7.16984C18.3386 6.83087 18.3086 6.30588 17.894 5.99723L12.525 2L7.15593 5.99723C6.74136 6.30588 6.7113 6.83087 7.08878 7.16984Z" fill="#304FFD"/>
                </svg>
                
            </div>
            <div>
              <h3 class="text-body font-normal text-base">Active</h3>
              <p class="text-[#3F434A] font-medium text-base">0</p>
            </div>
            </div>
        </LayoutPageCard>
      </div>
    </div>

    <div class="mt-5">
      <LayoutPageTable />
    </div>
  </div>


</template>
