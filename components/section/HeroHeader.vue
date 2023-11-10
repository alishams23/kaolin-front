



<template>
  <div class=" relative isolate overflow-hidden bg-white">
    <Navbar/>
    <svg class="absolute inset-0 -z-10 h-full w-full stroke-gray-200 [mask-image:radial-gradient(100%_100%_at_top_right,white,transparent)]" aria-hidden="true">
      <defs>
        <pattern id="0787a7c5-978c-4f66-83c7-11c213f99cb7" width="200" height="200" x="50%" y="-1" patternUnits="userSpaceOnUse">
          <path d="M.5 200V.5H200" fill="none" />
        </pattern>
      </defs>
      <rect width="100%" height="100%" stroke-width="0" fill="url(#0787a7c5-978c-4f66-83c7-11c213f99cb7)" />
    </svg>

    <div class="relative">
      <div class="mx-auto max-w-7xl">
        <div class="relative z-10 pt-14 lg:w-full lg:max-w-2xl">
          <svg class="absolute inset-y-0 right-8 hidden h-full w-80 translate-x-1/2 transform fill-white lg:block" viewBox="0 0 100 100" preserveAspectRatio="none" aria-hidden="true">
            <polygon points="0,0 90,0 50,100 0,100" />
          </svg>

          <div class="relative px-6 py-10 sm:py-40 lg:px-8 lg:py-56 lg:pr-0">
            <div class="mx-auto max-w-2xl lg:mx-0 lg:max-w-xl lg:flex-shrink-0 ">
              <div class="">
                <a href="#" class="inline-flex space-x-6">
                  <span class="rounded-full bg-red-600/10 px-3 py-1 text-sm font-semibold leading-6 text-red-600 ring-1 ring-inset ring-red-600/10">BHP company</span>
                 
                </a>
              </div>
              <h1 class="mt-10 text-4xl font-bold tracking-tight text-gray-900 sm:text-6xl">Kaolin</h1>
              <p class="mt-6 text-lg leading-8 text-gray-600">As the leading source of high-quality Kaolin, we proudly offer you top-grade Kaolin mineral. As a pioneering company in the mineral industry, we take pride in delivering our customers with unparalleled quality and high standards of Kaolin. Join us to experience our exceptional products and services.</p>
              <div class="mt-10 flex items-center gap-x-6">
                <a href="#" class="rounded-md bg-red-600 px-3.5 py-2.5 text-sm font-semibold text-white shadow-sm hover:bg-red-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-red-600">contact us</a>
                <a href="#" class="text-sm font-semibold leading-6 text-gray-900"> about Kaolin<span aria-hidden="true">→</span></a>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="bg-gray-50 lg:absolute lg:inset-y-0 lg:right-0 lg:w-1/2">
        <img class="aspect-[3/2] object-cover lg:aspect-auto lg:h-full lg:w-full" src="/photo/kaolin.jpg" alt="" />
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'
import { Dialog, DialogPanel } from '@headlessui/vue'
import { Bars3Icon, XMarkIcon } from '@heroicons/vue/24/outline'
import Navbar from '@/components/shared/Navbar.vue'

const navigation = [
  { name: 'Product', href: '#' },
  { name: 'Features', href: '#' },
  { name: 'Marketplace', href: '#' },
  { name: 'Company', href: '#' },
  { name: 'Log in', href: '#' },
]

const mobileMenuOpen = ref(false)
</script>