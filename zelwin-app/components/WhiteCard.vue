<template>
<div class="w-[343px]  bg-white rounded-[24px] mx-auto  md:w-[722px] md:pr-4  lg:w-[974px] xl:w-[1170px] 2xl:w-[1270px] px-[24px] py-[28px] md:px-[36px] md:py-[44px]" >
 <div class="text-[24px] flex font-bold md:text-[32px] md:font-extrabold lg:text-[44px]   "> ZELWIN STAKING APP </div>


<div class="md:flex md:justify-center  xl:flex xl:justify-between  ">
 <NiceButton class=" md:mt-[44px]  " >
      <template #header>
           <div class="text-left ">
               30 days

           </div>
       </template>
       <template #body1>
           <div  >
               
              APY:103,23%

           </div>
       </template> 
        <template #body2>
           <div >
               
               Amount:100-299ZLW

           </div>
       </template> 

 </NiceButton>

 <NiceButton class="mt-[15px]  md:mt-[44px] md:ml-[16px]" >
      <template #header>
           <div >
              90 days

           </div>
       </template>
       <template #body1>
           <div  >
               
              APY:103,23%

           </div>
       </template> 
        <template #body2>
           <div >
               
              Amount:100-299 ZLW

           </div>
       </template> 

 </NiceButton>

 <NiceButton class="mt-[16px]  md:mt-[44px] md:ml-[16px] " >
      <template #header>
           <div >
              150 days

           </div>
       </template>
       <template #body1>
           <div  >
               
              APY:103,23%

           </div>
       </template> 
        <template #body2>
           <div  >
            Amount:100-299 ZLW

           </div>
       </template> 

 </NiceButton>
 

</div>
<div class="flex w-[295px] bg-[#EFF3F8] rounded-[16px] mt-[28px] text-center md:w-[648px] lg:w-[886px] xl:w-[1058px] 2xl:w-[1058px]  ">
    
     <img src="../assets/svg/Informatıon.svg" alt="" class="w-[24px] h-[24px] mt-[16px] ml-[16.27px]  " >
     <p class="pt-[16px] pb-[16px] mr-[22px] md:pl-[20px] ">To perform actions on the page,connect your wallet</p>
    
     </div>



     <div class="md:flex md:justify-between ">
<ConnectButton >
      <template #header>
           <div class="bg-[#FFD42C] pt-[18px] pl-[86.5px] pb-[18px] pr-[86.5px] rounded-[12px] mt-[32px] md:mb-[32px]  ">
              Connect Wallet

           </div>
       </template>
    
     

</ConnectButton>
<ConnectButton >
      <template #header>
           <div class=" border-2 border-[#DFEBF5] pt-[18px] pl-[86.5px] pb-[18px] pr-[86.5px] rounded-[12px] mt-[20px] mb-[68px] md:mt-[44px] md:mb-[44px] md:justify-end ">
              View Contract

           </div>
       </template>
    
     

</ConnectButton>

</div>


</div>
</template>

<script>
import NiceButton from "./NiceButton.vue"
import ConnectButton from "./ConnectButton.vue"
export default {
    components : {
    NiceButton,
    ConnectButton
}
}
</script>