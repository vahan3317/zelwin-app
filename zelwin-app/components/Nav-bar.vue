<template>
 
 <div>
  <div class="flex justify-start items-center mx-auto px-[16px] py-[16px] md:justify-between md:mr-2    ">
      <div class="flex items-center justify-center xl:ml-28 ">
        <img class="w-[104px] h-[28px] md:ml-2 xl:  " src="../assets/svg/Group 3 (1).svg">
     
     </div>
       <button class="bg-white w-[153px]  rounded-xl flex justify-center pl-[15px] pt-[13px] pb-[13px] pr-[16px]  text-[16px]   lg:mr-2 xl:mr-28       " @click="toggleModall()">Connect Wallet</button>
    
  </div>

 </div>
</template>

<script>

export default {
 otherName: "modal",
  data(){
    return{
      showModal: false,
      isOpen: false,
    };
  },
  methods:{
    connectMetamask(){

// eslint-disable-next-line no-undef
ethereum.request({ method: 'eth_requestAccounts' });
      
    },
     toggleModall(){
      this.showModal = !this.showModal;
    }
   

  }
 
}
</script>
