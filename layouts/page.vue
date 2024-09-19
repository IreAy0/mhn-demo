<template>
      <div class="flex h-screen overflow-hidden">
        <LayoutPageSidebar />
        <div class="relative flex flex-1 flex-col overflow-y-auto overflow-x-hidden bg-[#F9FAFB]">
          <LayoutPageNavbar class="h-[64px] max-h-[64px] bg-slate-500" />
          <div class=" max-w-screen-2xl p-4 md:p-6 2xl:p-10 ">
              <slot />
          </div>
        </div>
      </div>
</template>
