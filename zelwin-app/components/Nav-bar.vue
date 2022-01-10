<template>
 
 <div>
  <div class="flex justify-between items-center px-[16px] py-[16px]">
      <div class="flex items-center justify-center">
        <img class="w-[104px] h-[28px] " src="../assets/svg/Group 3 (1).svg">
      </div>
       <button class="bg-white w-[153px] h-[44px] rounded-xl " @click="toggleModal = !toggleModal">Connect Wallet</button>
  </div>
 </div>
</template>

<script>
export default {
 otherName: "modal",
  data(){
    return{
      toggleModal:false,
      isOpen: false,
    };
  },
  methods:{
    connectMetamask(){

// eslint-disable-next-line no-undef
ethereum.request({ method: 'eth_requestAccounts' });
      
    }
   

  }
 
}
</script>
