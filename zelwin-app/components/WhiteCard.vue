<template>
<div class="  mt-[60px] w-[344.5px] px-[24px] py-[28px]  bg-white rounded-[24px] mx-auto  md:w-[722px] md:mx-auto   lg:w-[974px] xl:w-[1170px] xl:mx-auto   md:px-[36px] md:py-[44px]" >
 <div class="text-[24px] flex font-bold md:text-[32px] md:font-extrabold lg:text-[44px] xl:pl-[28px]      "> ZELWIN STAKING APP </div>


<div class=" mt-[29px] md:flex md:justify-around    ">
 <NiceButton class=" md:mt-[15px]  md:mr-[16px] xl:ml-[16px]    " >
      <template #header>
           <div class="  ">
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

 <NiceButton class="mt-[15px]  " >
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

 <NiceButton class=" mt-[15px] md:ml-[16px] lg:ml-[16px] xl:mr-[16px] " >
      <template #header>
           <div >
              150 days

           </div>
       </template>
       <template #body1>
           <div   >
               
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
<!-- <div class="flex w-[295px] bg-[#EFF3F8] rounded-[16px] mt-[28px]  md:w-[648px] lg:w-[886px] xl:w-[1058px] xl:ml-6  ">
    
     <img src="../assets/svg/Informatıon.svg" alt="" class="w-[24px] h-[24px] mt-[16px] ml-[16.27px]  " >
     <p class="pt-[16px] pb-[16px] mr-[22px] md:pl-[20px] text-[16px] text-[#828A97] ">To perform actions on the page,connect your wallet</p>
    
     </div> -->
<GrayDiv>
    <template #img>
        <div>
            <img src="../assets/svg/Informatıon.svg" alt="" >
        </div>
    </template>
      <template #text>
        <div>
            <p>To perform actions on the page,connect your wallet</p>
        </div>
    </template>
</GrayDiv>


     <div class="md:flex md:justify-between ">

 <div class="xl:pl-4">        
<ModalMeta>
       <template #button>
           <div class=" w-[295px]  bg-[#FFD42C] pt-[18px] pl-[86.5px] pb-[18px] pr-[88.5px] rounded-[12px] mt-[44px] md:mb-[32px]   " @click="toggleModal()">
Connect Wallet
           </div>

       </template>
       <template #modal>
           <div>
               
           </div>
       </template>
   </ModalMeta>



</div>
<ConnectButton class="xl:pr-4" >
      <template #header>
           <div class=" border-2 border-[#DFEBF5] pt-[18px] pl-[97.18px] pb-[18px] pr-[96.82px] rounded-[12px] mt-[20px] mb-[68px] md:mt-[44px] md:mb-[44px] md:justify-end ">
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
import GrayDiv from "./GrayDiv.vue";

export default {
    components : {
    NiceButton,
    ConnectButton,
    GrayDiv
},
methods:{
    connectMetamask(){

// eslint-disable-next-line no-undef
ethereum.request({ method: 'eth_requestAccounts' });
      
    },
     toggleModal() {
            this.showModal = !this.showModal;
        },
}
}
</script>
