<template>
 
 <div class="xl:border-b-2  xl:border-white xl:h-[88px] md:h-[68]  lg:border-b-2 lg:border-white md:border-b-2 md:border-white ">
  <div class="flex justify-between  items-center mx-auto px-[16px] py-[16px] md:justify-between md:w-[722px] lg:w-[974px]  xl:w-[1170px]    ">
      <div class="flex items-center  justify-center  ">
        <img class="min-w-[104px]      " src="../assets/svg/Group 3 (1).svg">
     
     </div>


   <ModalMeta>
       <template #button>
           <div class="flex justify-center items-center w-[164px] h-[48px]  bg-white rounded-lg md:ml-28     " @click="toggleModal()">
                Connect Wallet
           </div>

       </template>
       <template #modal>
           <div>
               
           </div>
       </template>
   </ModalMeta>

  </div>

 </div>

</template>

<script>

import ModalMeta from "./ModalMeta.vue";

export default {
    otherName: "showmodal",
    components: {  ModalMeta },
    data() {
        return {};
    },
    methods: {
        connectMetamask() {
            // eslint-disable-next-line no-undef
            ethereum.request({ method: "eth_requestAccounts" });
        },
        toggleModal() {
            this.showModal = !this.showModal;
        },
    }
}
</script>
