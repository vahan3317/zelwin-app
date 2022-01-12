<template>
  <div>
    
   <ConnectButton >
      <template #header>
           <div class="bg-[#FFD42C] pt-[18px] pl-[86.5px] pb-[18px] pr-[86.5px] rounded-[12px] mt-[44px] md:mb-[32px]  "   @click="toggleModal()">
              Connect Wallet

           </div>
       </template>
    
     

</ConnectButton>
    <div v-if="showModal" class="overflow-x-hidden overflow-y-auto fixed inset-0 z-50 outline-none focus:outline-none justify-center items-center flex  ">
      <div class="relative w-auto my-6 mx-auto max-w-3xl w-[630px] rounded-[24px] ">
        <!--content-->
        <div class="border-0 rounded-lg shadow-lg relative flex flex-col w-full bg-white outline-none focus:outline-none">
          <!--header-->
          <div class="flex items-start justify-between   border-solid border-blueGray-200 rounded-t">
           
            
          </div>
           <div class="relative  flex-auto">
            <button class="p-1 ml-auto bg-transparent border-0 text-black  float-right text-3xl leading-none font-semibold outline-none focus:outline-none" @click="toggleModal()">
              <span class="bg-transparent text-black  w-[44px] h-[44px]  block outline-none focus:outline-none">
                X
              </span>
            </button>
            <p class=" md:text-[16px] font-bold  xl:text-[24px] leading-relaxed pt-[61px] max-w-[423px] md:pl-[56px] ">
             Select the payment card that you want to use for paymant
            </p>
          </div>
          <!--body-->
          <div class="relative flex-auto md:mt-[32px] md:pl-[56px]">
            <p class="  ">
             The selected Wallet will be connected to your staking
            </p>
          </div>
          
          
          <div class="flex">
           <div class="flex md:mt-[24px] md:ml-[56px]  md:h-[108px] xl:mb-[50px]  md:w-[271px] md:pl-[57px] md:pt-[32px] md:mb-[32px] rounded-xl md:ml-4   text-center items-center p-3 border-2 border-gray-300 font-bold hover:text-white hover:bg-gray-300 md:w-32 md:h-12 " @click="connectMetamask" >
                                    <img
src="https://upload.wikimedia.org/wikipedia/commons/3/36/MetaMask_Fox.svg"
                                              class="w-[44px] ">
                                                Metamask
                                            </div>
                                             <div class="flex md:mt-[24px] md:mr-[56px]  md:ml-[56px]  md:h-[108px] xl:mb-[50px]  md:w-[271px] md:pl-[57px] md:pt-[32px] md:mb-[32px] rounded-xl md:ml-4   text-center items-center p-3 border-2 border-gray-300 font-bold hover:text-white hover:bg-gray-300 md:w-32 md:h-12 " @click="connectMetamask" >
                                    <img
src="https://upload.wikimedia.org/wikipedia/commons/3/36/MetaMask_Fox.svg"
                                              class="w-[44px] ">
                                                Metamask
                                            </div>
                                            </div>
        
        </div>
      </div>
    </div>
    <div v-if="showModal" class="opacity-25 fixed inset-0 z-40 bg-black"></div>
  </div>
</template>

<script>
export default {
  name: "ModalComponent",
  data() {
    return {
      showModal: false
    }
  },
  methods: {
    toggleModal(){
      this.showModal = !this.showModal;
    }
  }
}
</script>
