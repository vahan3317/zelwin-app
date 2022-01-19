<template>
<div class="flex flex-col  mt-[60px] mb-[28px] w-[344.5px] px-[26px] pt-[28px]  md:pt-[44px] md:px-[36px] lg:pt-[56px] lg:px-[44px] xl:pt-[64px] xl:px-[56px]  bg-white rounded-[24px] mx-auto  md:w-[722px] md:mx-auto   lg:w-[974px] xl:w-[1170px] xl:mx-auto   md:px-[36px] md:py-[44px]" >
 <div class="text-[24px] flex  font-bold md:text-[32px] md:font-extrabold lg:text-[44px]  font-['Montserrat']     "> ZELWIN STAKING APP </div>


<div class=" mt-[29px]   flex  flex-col justify-between md:flex md:flex-row       ">
 <NiceButton class=" mt-[15px]     " >
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

 <NiceButton class="mt-[15px] md:ml-[16px] lg:ml-[26px] xl:ml-[32px]   " >
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

 <NiceButton class=" mt-[15px] md:ml-[16px] lg:ml-[26px]   " >
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

<GrayDiv class="">
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


     <div class=" mt-[24px] md:mt-[44px] pb-[68px] md:pb-[44px] lg:pb-[56px] xl:pb-[64px] md:flex md:justify-between  ">

      
<ModalMeta>
       <template #button>
           <div class=" flex justify-center items-center w-[295px] h-[56px]  bg-[#FFD42C]  rounded-[12px]  text-white md:w-[230px] font-bold   " @click="toggleModal()">
Connect Wallet
           </div>

       </template>
       <template #modal>
           <div>
               
           </div>
       </template>
   </ModalMeta>




<ConnectButton  >
      <template #header>
           <div class="flex justify-center items-center mt-[20px] md:mt-0 w-[295px] h-[56px] border-2 border-[#DFEBF5]   rounded-[12px]      md:w-[230px]  ">
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
