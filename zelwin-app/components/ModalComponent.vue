<template>
  <div>
    
   <ConnectButton >
      <template #header>
           <div class="bg-[#FFD42C] pt-[18px] pl-[86.5px] pb-[18px] pr-[86.5px] rounded-[12px] mt-[44px] md:mb-[32px]  "   @click="toggleModal()">
              Connect Wallet

           </div>
       </template>
    
     

</ConnectButton>
    <div v-if="showModal" class="overflow-x-hidden overflow-y-auto fixed inset-0 z-50 outline-none focus:outline-none justify-center items-center flex  " @click="toggleModal()">
      <div class="relative   my-6 mx-auto  ">
        <!--content-->
        <div class="min-w-[343px] border-px mx-auto md:w-[630px]   relative flex flex-col w-full bg-white outline-none focus:outline-none rounded-[24px] lg:w-[646px] ">
          <!--header-->
          <div class="flex items-end justify-between   ">
           
            
          </div>
           <div class="relative  flex-auto">
            <button class=" p-4  bg-transparent float-right    leading-none font-semibold outline-none focus:outline-none" @click="toggleModal()">
              <span class="bg-transparent     block outline-none focus:outline-none" @click="toggleModal()">
               <img src="../assets/svg/close.svg" alt=""  class="">
              </span>
            </button>
            <p class=" md:text-[16px] pt-[61px] pl-[56px] max-w-[423px] font-bold  xl:text-[24px] leading-relaxed pt-[61px]   md:pl-[56px] ">
             Select the payment card that  you want to use for paymant
            </p>
          </div>
          <!--body-->
          <div class="relative flex-auto pt-[32px] pl-[56px] ">
            <p class="  max-w-[295px] ">
             The selected Wallet will be connected to your staking
            </p>
          </div>
          
          
          <div class="flex   xl:mt-[24px]   md:mt-[24px] mt-[24px]  ">
           <div class="flex ml-[56px] pt-[36px] pb-[32px]   mb-[56px] pl-[57px] pr-[57px] w-[273px] border-2 rounded-[12px]  md:mr-[56px]        hover:bg-gray-300 "  @click="connectMetamask()" >
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
