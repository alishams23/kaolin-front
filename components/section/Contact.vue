
<template>
    <div class="relative isolate bg-gray-900" id="contact">
      <div class="mx-auto  grid max-w-7xl grid-cols-1 lg:grid-cols-2">
        <div class="relative px-6 pb-20 pt-24 sm:pt-32 lg:static lg:px-8 ">
          <div class="mx-auto max-w-xl lg:mx-0 lg:max-w-lg">
            <div class="absolute inset-y-0 left-0 -z-10 w-full overflow-hidden  border-r border-gray-800   lg:w-1/2">
              <svg class="absolute inset-0 h-full w-full stroke-gray-700 [mask-image:radial-gradient(100%_100%_at_top_right,white,transparent)]" aria-hidden="true">
                <defs>
                  <pattern id="54f88622-e7f8-4f1d-aaf9-c2f5e46dd1f2" width="200" height="200" x="100%" y="-1" patternUnits="userSpaceOnUse">
                    <path d="M130 200V.5M.5 .5H200" fill="none" />
                  </pattern>
                </defs>
                <svg x="100%" y="-1" class="overflow-visible fill-gray-800/20">
                  <path d="M-470.5 0h201v201h-201Z" stroke-width="0" />
                </svg>
                <rect width="100%" height="100%" stroke-width="0" fill="url(#54f88622-e7f8-4f1d-aaf9-c2f5e46dd1f2)" />
              </svg>
           
            </div>
            <h2 class="text-3xl font-bold tracking-tight text-white">Get in touch</h2>
            <p class="mt-6 text-lg leading-8 text-gray-300">You can contact us via the information provided below or by filling out the contact form. We appreciate your interest in our products and look forward to connecting with you.</p>
            <dl class="mt-10 space-y-4 text-base leading-7 text-gray-300">
            
              <div class="flex gap-x-4">
                <dt class="flex-none">
                  <span class="sr-only">Email</span>
                  <EnvelopeIcon class="h-7 w-6 text-gray-400" aria-hidden="true" />
                </dt>
                <dd><a class="hover:text-white" href="mailto:info@bhp-kaolin.com">info@bhp-kaolin.com</a></dd>
              </div>
              <div class="flex gap-x-4">
                <dt class="flex-none">
                  <span class="sr-only">Email</span>
                  <EnvelopeIcon class="h-7 w-6 text-gray-400" aria-hidden="true" />
                </dt>
                <dd><a class="hover:text-white" href="mailto:sales@bhp-kaolin.com">sales@bhp-kaolin.com</a></dd>
              </div>
            </dl>
          </div>
        </div>
        <form action="#" method="POST" class="px-6 pb-24 pt-20 sm:pb-32 lg:px-8 ">
          <div class="mx-auto max-w-xl lg:mr-0 lg:max-w-lg">
            <div class="grid grid-cols-1 gap-x-8 gap-y-6 sm:grid-cols-2">
              <div>
                <label for="first-name" class="block text-sm font-semibold leading-6 text-white">First name</label>
                <div class="mt-2.5">
                  <input type="text" name="first-name" id="first-name" autocomplete="given-name" class="block w-full rounded-md border-0 bg-white/5 px-3.5 py-2 text-white shadow-sm ring-1 ring-inset ring-white/10 focus:ring-2 focus:ring-inset focus:ring-red-500 sm:text-sm sm:leading-6" />
                </div>
              </div>
              <div>
                <label for="last-name" class="block text-sm font-semibold leading-6 text-white">Last name</label>
                <div class="mt-2.5">
                  <input type="text" name="last-name" id="last-name" autocomplete="family-name" class="block w-full rounded-md border-0 bg-white/5 px-3.5 py-2 text-white shadow-sm ring-1 ring-inset ring-white/10 focus:ring-2 focus:ring-inset focus:ring-red-500 sm:text-sm sm:leading-6" />
                </div>
              </div>
              <div class="sm:col-span-2">
                <label for="email" class="block text-sm font-semibold leading-6 text-white">Email</label>
                <div class="mt-2.5">
                  <input type="email" name="email" id="email" autocomplete="email" class="block w-full rounded-md border-0 bg-white/5 px-3.5 py-2 text-white shadow-sm ring-1 ring-inset ring-white/10 focus:ring-2 focus:ring-inset focus:ring-red-500 sm:text-sm sm:leading-6" />
                </div>
              </div>
           
              <div class="sm:col-span-2">
                <label for="message" class="block text-sm font-semibold leading-6 text-white">Message</label>
                <div class="mt-2.5">
                  <textarea name="message" id="message" rows="4" class="block w-full rounded-md border-0 bg-white/5 px-3.5 py-2 text-white shadow-sm ring-1 ring-inset ring-white/10 focus:ring-2 focus:ring-inset focus:ring-red-500 sm:text-sm sm:leading-6" />
                </div>
              </div>
            </div>
            <div class="mt-8 flex justify-end">
              <button type="submit" class="rounded-md bg-red-500 px-3.5 py-2.5 text-center text-sm font-semibold text-white shadow-sm hover:bg-red-400 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-red-500">Send message</button>
            </div>
          </div>
        </form>
      </div>
    </div>
  </template>
  
  <script setup>
  import {  EnvelopeIcon } from '@heroicons/vue/24/outline'
  </script>