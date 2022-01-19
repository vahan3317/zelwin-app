<template>
  <div class=""
    >
    <button class="flex justify-center  "  @click="toggleModal()"  ><slot name="button">  </slot></button>
    <div v-if="showModal"  >
     
    
    <div  class=" flex flex-col  fixed inset-0 z-50 justify-center     " @click="toggleModal()">
      
        
        <div class=" relative min-w-[343px] px-[24px]  pt-[28px] pb-[28px]   bg-white  border-px mx-auto md:w-[630px]     rounded-[24px] lg:w-[646px] lg:h-[352px]  xl:w-[670px] xl:h-[352px] xl:px-[56px] xl:pt-[61px]    ">
      
          
           
              <button class="absolute right-[20px] top-[2px]  lg:top-[20px]    " @click="toggleModal()">
              
               <img src="../assets/svg/close.svg" alt=""  @click="toggleModal()">
             
            </button>
           
           <div class=" max-w-[423px]   text-[24px] font-extrabold  ">
             Select the payment card that  you want to use for payment
           </div>
                     
          
          <div class="w-[295px] mt-[32px] md:w-auto  text-[16px]       ">
            
             The selected Wallet will be connected to your staking
            
          </div>
          
          
          
                      <div class=" mx-auto flex justify-center  items-center  w-[295px] h-[108px]  md:w-[230px]   mt-[24px]       border-2 rounded-[12px]        hover:bg-gray-300 "  @click="connectMetamask()" >
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