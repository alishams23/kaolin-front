<template>
    <div class="  bg-white pb-10 sm:pb-10" id="aboutUs">
      <div aria-hidden="true" class="relative">
        <img src="/photo/mine.webp" alt="" class="h-96 w-full object-cover object-center" />
        <div class="absolute inset-0 bg-gradient-to-t from-white" />
      </div>
  
      <div class="relative mx-auto -mt-24 max-w-7xl px-4 pb-16 sm:px-6 sm:pb-24 lg:px-8">
        <div class="mx-auto max-w-2xl lg:text-center">
          <h2 class="text-base font-semibold leading-7 text-red-600">benefits</h2>
          <p class="mt-2 text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">Why Choose Us ?</p>
          <p class="mt-6 text-lg leading-8 text-gray-600">
            
            Discover the advantages of partnering with us, a leading force in the mining industry. With decades of experience, we stand out for our commitment to excellence, innovation, and quality. Our diverse product portfolio, ranging from valuable raw materials to meticulously crafted final products, caters to the unique needs of various industries, making us a versatile and reliable choice.
<br>
<br>
Explore the exceptional benefits of our standout product, Kaolin, renowned for its versatile applications in construction, ceramics, healthcare, and cosmetics. Produced using cutting-edge technologies and professional processing techniques, our Kaolin consistently meets and exceeds global standards.
          </p>
        </div>
        <div class="mx-auto mt-16 max-w-2xl sm:mt-20 lg:mt-24 lg:max-w-4xl">
          <dl class="grid max-w-xl grid-cols-1 gap-x-8 gap-y-10 lg:max-w-none lg:grid-cols-2 lg:gap-y-16">
            <div v-for="feature in features" :key="feature.name" class="relative pl-16">
              <dt class="text-base font-semibold leading-7 text-gray-900">
                <div class="absolute left-0 top-0 flex h-10 w-10 items-center justify-center rounded-lg bg-red-600">
                  <component :is="feature.icon" class="h-6 w-6 text-white" aria-hidden="true" />
                </div>
                {{ feature.name }}
              </dt>
              <dd class="mt-2 text-base leading-7 text-gray-600">{{ feature.description }}</dd>
            </div>
          </dl>
        </div>
      </div>
    </div>
  </template>
  
  <script setup>
  import { UserGroupIcon, StarIcon,  } from '@heroicons/vue/24/outline'
  
  const features = [
    {
      name: 'Commitment to Quality',
      description:
        'We are dedicated to maintaining high quality from extraction to distribution.',
      icon: StarIcon,
    },
    {
      name: 'Specialized Team',
      description:
        'Our team is comprised of knowledgeable and committed individuals.',
      icon: UserGroupIcon,
    },

  ]
  </script>