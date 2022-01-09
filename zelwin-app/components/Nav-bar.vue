<template>
 
 <div class="container">
  
  <header class=" flex justify-between  mx-auto  px-4 py-3 pl-2 md:pr-6 xl:mx-auto xl:pr-24      ">
    <div class="flex items-center justify-between mx-auto px-4 py-3 sm:p-0 xl:pr-44 ">
      <div>
        <p><img class="w-[204px] h-[28px] md:pr-24 lg:mr-56   xl:-pl-24  " src="../assets/svg/Group 3 (1).svg"  alt=""></p>
      </div>
       <button class="sm:hidden ml-36 bg-white   w-[153px] h-[44px] rounded-xl  " @click="toggleModal = !toggleModal">Connect Wallet</button>
      <div class="sm:hidden">
   

        <button type="button" class="block text-gray-500 hover:text-white focus:text-white focus:outline-none" @click="isOpen = !isOpen">
          <svg class="h-8 w-8 ml-px fill-current" viewBox="0 0 24 24">
            <path v-if="isOpen" fill-rule="evenodd" d="M18.278 16.864a1 1 0 0 1-1.414 1.414l-4.829-4.828-4.828 4.828a1 1 0 0 1-1.414-1.414l4.828-4.829-4.828-4.828a1 1 0 0 1 1.414-1.414l4.829 4.828 4.828-4.828a1 1 0 1 1 1.414 1.414l-4.828 4.829 4.828 4.828z"/>
            <path v-if="!isOpen" fill-rule="evenodd" d="M4 5h16a1 1 0 0 1 0 2H4a1 1 0 1 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2z"/>
          </svg>
        </button>
      </div>
    </div>
    
    <nav :class="isOpen ? 'block' : 'hidden'" class="px-2 pt-2 pb-4 sm:flex sm:p-0 md:ml-24  lg:pl-6 xl:w-auto xl:-mr-10     ">
      <a href="#" class="block px-2 py-2 text-black font-semibold rounded hover:border-b-2 hover:border-red-600 hover:-mt-2 hover:text-red-600">Stacking</a>
      <a href="#" class="mt-1 block px-2 py-2 text-black font-semibold rounded hover:border-b-2 hover:border-red-600  hover:-mt-2 sm:mt-0 sm:ml-2 hover:text-red-600">ZlW bridge</a>
      <a href="#" class="mt-1 block px-2 py-2 text-black font-semibold rounded hover:border-b-2 hover:border-red-600  hover:-mt-2 sm:mt-0 sm:ml-2 hover:text-red-600">SHO</a>
      <a  class="mt-1  block px-4 py-2 text-black bg-white w-[155px] h-[44px] font-semibold rounded hover:bg-gray-300 sm:mt-0 sm:ml-2" @click="toggleModal = !toggleModal">Connect Wallet</a>
    
    </nav>
  </header>
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
