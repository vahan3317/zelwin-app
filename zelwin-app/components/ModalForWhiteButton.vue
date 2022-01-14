<template>
  <div class="xl:mr-24  ">
    
   <ConnectButton >
      <template #header>
           <div class=" w-[164px] ml-16 pl-[25px]  pt-[14px] pr-[25.63px]  pb-[14px] bg-white rounded-lg md:ml-28    "   @click="toggleModal()">
              Connect Wallet

           </div>
       </template>
    
     

</ConnectButton>
    <div v-if="showModal" class="overflow-x-hidden overflow-y-auto fixed inset-0 z-50 outline-none focus:outline-none justify-center items-center flex  " @click="toggleModal()">
      <div class="relative w-auto h-auto  my-6 mx-auto  md:w-[630px] md:h-[365px]  ">
        <!--content-->
        <div class="border-0 rounded-lg shadow-lg relative flex flex-col w-full bg-white outline-none focus:outline-none rounded-[24px]">
          <!--header-->
          <div class="flex items-start justify-between   border-solid border-blueGray-200 rounded-t">
           
            
          </div>
           <div class="relative  flex-auto">
            <button class="p-1 ml-auto bg-transparent border-0 text-black  float-right text-3xl leading-none font-semibold outline-none focus:outline-none" @click="toggleModal()">
              <span class="bg-transparent text-gray-300  w-[44px] h-[44px]  block outline-none focus:outline-none" @click="toggleModal()">
                X
              </span>
            </button>
            <p class=" md:text-[16px] font-bold  xl:text-[24px] leading-relaxed pt-[61px] max-w-[423px]  md:pl-[56px] ">
             Select the payment card that that <br> you want to use for paymant
            </p>
          </div>
          <!--body-->
          <div class="relative flex-auto md:mt-[32px] md:pl-[56px]">
            <p class="  ">
             The selected Wallet will be connected to your staking
            </p>
          </div>
          
          
          <div class="flex   xl:mt-[24px]  md:ml-[56px] md:mt-[24px] mt-[24px]  ">
           <div class="flex  mb-[56px] pl-[57px] pr-[57px] xl:w-[273px] border-2 md:mb-[56px] md:items-center md:pr-[56px] md:pt-[32px] md:pb-[32px]  md:pl-[57px]     xl:pl-[57px] xl:mb-[56px] xl:pt-[32px] xl:pb-[32px] xl:mb-[56px] xl:rounded-lg hover:bg-gray-300 "  @click="connectMetamask()" >
                                    <img
src="https://upload.wikimedia.org/wikipedia/commons/3/36/MetaMask_Fox.svg"
                                              class="w-[44px] ">
                                                Metamask
                                            </div>
                                           <div class="flex ml-[16px] pr-[57px] mb-[57px] pl-[57px] mb-[50px]  md:mb-[56px] md:pl-[57px] md:pr-[56px] md:items-center md:ml-[16px]  xl:w-[273px] border-2  xl:pt-[32px]  xl:mb-[56px] xl:pb-[32px] xl:mb-[56px] xl:pl-[57px] xl:mr-[56px] xl:ml-[16px] xl:rounded-lg hover:bg-yellow-300  " @click="connectMetamask()" >
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
    },
    connectMetamask(){

// eslint-disable-next-line no-undef
ethereum.request({ method: 'eth_requestAccounts' });
      
    },
  }
}
</script>
