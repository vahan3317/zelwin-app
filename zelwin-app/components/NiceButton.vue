<template>
  <button
    class="flex flex-col w-[295px]  md:min-w-[206px]  lg:w-[278px] xl:w-[331px]     border-2 border-[#DFEBF5]  rounded-[24px]   hover:bg-[#EFF3F8] xl:w-[331px]      ">
    <div class="font-bold text-[28px]   pt-[16px] pl-[20px]  md:text-[28px]    xl:pl-[24px]  xl:text-[36px]  xl:pl-[28px]    "><slot name="header"> </slot></div>
    <div class="text-[#DA554A]  pt-[8px] text-[16px] font-semibold  pl-[20px] md:text-[16px] xl:text-[20px]  xl:pl-[28px]    "><slot name="body1"> </slot></div>
    <div class="text-[14px] pt-[12px]  text-[#828A97] pb-[16px] lg:pb-[20px]  pl-[20px]  md:text-[14px] xl:text-[20px] xl:pl-[28px]   "><slot name="body2"> </slot></div>
    <slot> </slot>
  </button>
</template>

<script>
export default {}
</script>

<style></style>
