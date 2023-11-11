<template>
  <div class="mx-auto  mb-[15rem] max-w-7xl  sm:px-6 lg:px-8" id="attachment">
    <div class="relative isolate overflow-hidden bg-gray-900 px-6 py-24 text-center shadow-2xl sm:rounded-3xl sm:px-16">
      <h2 class="mx-auto max-w-2xl text-3xl font-bold tracking-tight text-white sm:text-4xl">Products</h2>
      <div class="mt-10" v-if="loading == true">
        <div
          class="inline-block h-10 w-10 animate-spin rounded-full border-4 border-solid border-current border-r-transparent align-[-0.125em] text-neutral-100 motion-reduce:animate-[spin_1.5s_linear_infinite]"
          role="status">
          <span
            class="!absolute !-m-px !h-px !w-px !overflow-hidden !whitespace-nowrap !border-0 !p-0 ![clip:rect(0,0,0,0)]">Loading...</span>
        </div>
      </div>
      <div
      v-for=" item in data"

        class="mx-auto mt-10 flex justify-between max-w-2xl flex-col gap-16 bg-white/5 px-6 py-16 ring-1 ring-white/10 sm:rounded-3xl sm:p-8 lg:mx-0 lg:max-w-none lg:flex-row lg:items-center lg:py-10 xl:gap-x-10 xl:px-10mx-auto flex max-w-2xl flex-col gap-16 bg-white/5 px-6 py-16 ring-1 ring-white/10 sm:rounded-3xl sm:p-8 lg:mx-0 lg:max-w-none lg:flex-row lg:items-center lg:py-10 xl:gap-x-10 xl:px-10">
        <div class="text-white ">
          {{ item.title }}
        </div>
        <a :href="item.file"
        download="file"
          class="text-white bg-red-700 hover:bg-red-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center inline-flex items-center me-2 ">
          <ArrowDownTrayIcon class="h-4 pr-3" />
          download
        </a>
      </div>

      <svg
        class="absolute inset-0 -z-10 h-full w-full stroke-gray-700 [mask-image:radial-gradient(100%_100%_at_bottom_left,white,transparent)]"
        aria-hidden="true">
        <defs>
          <pattern id="0787a7c5-978c-4f66-83c7-11c213f99cb7" width="200" height="200" x="50%" y="-1"
            patternUnits="userSpaceOnUse">
            <path d="M.5 200V.5H200" fill="none" />
          </pattern>
        </defs>
        <rect width="100%" height="100%" stroke-width="0" fill="url(#0787a7c5-978c-4f66-83c7-11c213f99cb7)" />
      </svg>
    </div>
  </div>
</template>



<script>
import { ArrowDownTrayIcon, } from '@heroicons/vue/24/outline'

export default {

  components: {
    ArrowDownTrayIcon
  },
  data() {
    return {
    loading:true,
      data:[]
   
    };
  },
  methods: {
    async getData(){

     await fetch(
        `http://127.0.0.1:8000/api/files/FilesList/`,
        {
          headers: {
            "Content-type": "application/json",
            Accept: "application/json",
          },
        }
      )
        .then((response) => response.json())
        .then((data) => {
          this.data = data;
          this.loading = false;
        });



    }
  
  }, 
  mounted() {
    // this.getDataHome(this.postPage);
    this.getData()
    
  },
};

</script>

<style></style>