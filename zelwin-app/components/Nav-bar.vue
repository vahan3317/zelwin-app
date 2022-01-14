<template>
 
 <div class="xl:border-b-2  xl:border-white xl:h-[88px] md:h-[68]  lg:border-b-2 lg:border-white md:border-b-2 md:border-white ">
  <div class="flex justify-between w-auto items-center mx-auto px-[16px] py-[16px] md:justify-between md:mr-2    ">
      <div class="flex items-center  justify-center xl:ml-28 ">
        <img class="min-w-[104px]    md:ml-2 :  " src="../assets/svg/Group 3 (1).svg">
     
     </div>
      <!-- <button class="bg-white w-[153px]  rounded-xl flex justify-center pl-[15px] pt-[13px] pb-[13px] pr-[16px]  text-[16px]   lg:mr-2 xl:mr-28       " @click="toggleModal()">Connect Wallet</button> -->
    <ModalForWhiteButton  class=""></ModalForWhiteButton>
  </div>

 </div>
</template>

<script>
import ModalForWhiteButton from "./ModalForWhiteButton.vue";

export default {
    otherName: "showmodal",
    components: { ModalForWhiteButton },
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
