<template>
  <div class="xl:mr-4"
    >
    <button @click="toggleModal()" ><slot name="button"> Connect Wallet </slot></button>
    <div v-if="showModal"  >
     
    
    <div  class="flex flex-col  fixed inset-0 z-50 justify-center  mx-auto  flex  " @click="toggleModal()">
      
        
        <div class=" min-w-[343px] min-h-[332px] bg-white  border-px mx-auto md:w-[630px]     rounded-[24px] lg:w-[646px] lg:h-[352px]  xl:w-[670px] xl:h-[352px]  ">
      
          
           <div class="   ">
            <button class=" p-[16px] float-right   " @click="toggleModal()">
              
               <img src="../assets/svg/close.svg" alt=""  @click="toggleModal()">
             
            </button>
           <div class="pt-[61px] pl-[24px] md:pl-[36px] max-w-[423px]  text-[24px] font-extrabold  ">
             Select the payment card that  you want to use for paymant
           </div>
                     </div>
          
          <div class="w-[295px] mt-[32px] md:w-auto pl-[24px] text-[16px]  md:pl-[36px]     ">
            
             The selected Wallet will be connected to your staking
            
          </div>
          
          
         
           <div class="flex justify-center w-[295px] mb-[56px] md:w-[230px]  items-center mt-[24px]  ml-[24px] pt-[34px] pb-[32px]    pl-[57px] pr-[57px]  border-2 rounded-[12px]  md:ml-[32px] md:mb-[56px]        hover:bg-gray-300 "  @click="connectMetamask()" >
                                    <img
src="https://upload.wikimedia.org/wikipedia/commons/3/36/MetaMask_Fox.svg"
                                              class="w-[44px] h-[44px] ">
                                     <div >Metamask</div>          
                                            </div>
                                  
                                         
        
        </div>
      
    </div>
    <div v-if="showModal" class="opacity-30 fixed inset-0 z-40 bg-black"></div>
     
     
     </div>
   
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

<style></style>