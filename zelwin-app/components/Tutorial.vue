<!-- Please remove this file from your project -->
<template>
<div>

<div class=" w-[343px] h-[843px] ml-4  bg-white rounded md:mx-auto   md:w-[722px] md:h-[525px]  lg:mx-auto lg:w-[974px] lg:h-[579px] xl:mx-auto xl:w-[1170px] xl:h-[634] 2xl:w-[1270px] h-[634px]    " >
  
  <div class="ml-[20px] md:flex md:flex-row md:pt-8 md:pl-2 xl:ml-28      ">
    <p class="font-bold text-[24px] md:text-[32px]  lg:text-[44px]    ">
    Zelwin 
    </p>
      <p class="font-bold text-[24px] md:pl-2  md:text-[32px]   lg:text-[44px]  ">
       Stacking 
      </p>
       <p class="font-bold text-[24px] md:pl-2  md:text-[32px]   lg:text-[44px] ">
        App
      </p>
  </div>

  <div class="md:flex md:flex-row md:mx-auto md:pt-12 xl:ml-36" >
       <div class="w-[295px]  h-[133px] ml-[20px] mt-2 border-2 rounded-xl hover:bg-gray-200   lg:w-[278px] lg:h-[147px] ">
         <h1 class="ml-[20px] mt-[20px]  lg: text-[32px] xl:text-[36px]">30 Days</h1>
         <h2 class="ml-[20px] lg:text-[18px] xl:text-[20px]" >APY:103.23%</h2>
         <h3 class="ml-[20px] lg:text-[18px] xl:text-[20px]">Amount:100-299ZLW</h3>
       </div>
         <div class="w-[295px]  h-[133px] ml-[20px] mt-2 border-2 rounded-xl hover:bg-gray-200  lg:w-[278px] lg:h-[147px] ">
         <h1 class="ml-[20px] mt-[20px] lg:text-[32px] xl:text-[36px] ">90 Days</h1>
         <h2 class="ml-[20px] lg:text-[18px] xl:text-[20px]">APY:103.23%</h2>
         <h3 class="ml-[20px] lg:text-[18px] xl:text-[20px]">Amount:100-299ZLW</h3>
       </div>
         <div class="w-[295px]  h-[133px] ml-[20px] mt-2 border-2 rounded-xl hover:bg-gray-200 lg:w-[278px] lg:h-[147px] ">
         <h1 class="ml-[20px] mt-[20px] lg:text-[32px] xl:text-[36px]">150 Days</h1>
         <h2 class="ml-[20px] lg:text-[18px] xl:text-[20px]">APY:103.23%</h2>
         <h3 class="ml-[20px] lg:text-[18px] xl:text-[20px]">Amount:100-299ZLW</h3>
       </div>
  </div>
  
  <div>
    <img src="../assets/svg/Group 33547.svg" class="w-[648px] h-[72px] hidden md:block  md:ml-[40px] md:mt-[20px] lg:w-[886px] lg:h-[72px] xl:w-[1258px] xl:mx-auto 2xl:w-[1058px]  " alt="">
  </div>
  <div>
    <button
    class="ml-4 mb-12 bg-yellow-300 font-sans font-semibold shadow-lg  xl:mt-8 xl:ml-36  hover:bg-yellow-400  " @click="toggleModal = !toggleModal">Connect Wallet</button> 
    <div v-if="toggleModal" class="fixed mt-2 overflow-y-auto inset-24 flex justify-center items-center z-50">
    <div class="relative   mx-auto ">
       <div 
      class="fixed inset-12 mx-auto  z-20  bg-opacity-300 duration-300 overflow-y-auto "
      x-show=" showModal"
      x-transition:enter="transition duration-300"
      x-transition:enter-start="opacity-0"
      x-transition:enter-end="opacity-100"
      x-transition:leave="transition duration-300"
      x-transition:leave-start="opacity-100"
      x-transition:leave-end="opacity-0"
       @click="toggleModal=false"
    >
      <div class="w-[343px] relative  mt-72 mr-24  modal mx-2 mx-auto my-10 opacity-300  md:w-[630px] md:h-[340px] md:ml-8 lg:w-[646px] lg:h-[372px]  lg:ml-32 xl:ml-[670px] xl:ml-[388px] 2xl:w-[670px] 2xl:h-[365px] 2xl:ml-[800px] " @click="toggleModal=false" >
        <div
          class="relative bg-gray-100 shadow-lg rounded-2xl text-gray-900 z-20 "
          x-show="showModal1"
          x-transition:enter="transition transform duration-300"
          x-transition:enter-start="scale-0"
          x-transition:enter-end="scale-100"
          x-transition:leave="transition transform duration-300"
          x-transition:leave-start="scale-100"
          x-transition:leave-end="scale-0"
          @click="showModal = false"
        >
          <header class="flex   md:ml-[340px] mb-2  " >
            <!-- <h2 class="font-semibold">Locked Stacking</h2> -->
            <button class="focus:outline-none ml-72  md:ml-64   " @click="toggleModal=false">
              <svg class="fill-current" xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 18 18">
                <path
                  d="M14.53 4.53l-1.06-1.06L9 7.94 4.53 3.47 3.47 4.53 7.94 9l-4.47 4.47 1.06 1.06L9 10.06l4.47 4.47 1.06-1.06L10.06 9z"
                ></path>
              </svg>
            </button>
          </header>
          <div class="flex-auto  bg-gray-100  rounded-2xl  ">
          
                           <div class="container    ">
                             <p class="font-bold  text-lg text-left md:ml-4 md: lg:text-xl  ">Select the payment card that <br> you want to use for payment</p><br>
                             <p class="text-gray-400 text-left  md:ml-4">The selected wallet will be your stacking </p>
                             
                             <div
                                   class="flex butMeta w-36 h-12  rounded-xl md:ml-4   text-center items-center p-3 border-2 border-gray-300 font-bold hover:text-white hover:bg-gray-300 md:w-32 md:h-12 "
                          @click="connectMetamask"
                                   
                                   >
                                    <img
                                        src="https://upload.wikimedia.org/wikipedia/commons/3/36/MetaMask_Fox.svg" alt="Metamask"
                                              class="h-5 mr-2">
                                                Metamask
                                            </div>
                          </div>
                       </div>



                    
            </div>
          </div>
        </div>
      </div>
    </div>

    </div></div>
 <div v-if="toggleModal" class="  absolute inset-0 z-40 w-full  opacity-25 bg-black"></div>
  
    
  


</div>









</template>

<script>

export default {
  name: 'NuxtTutorial',
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