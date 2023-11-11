<template>
    <div class="bg-white py-24 sm:py-32">
      <div class="mx-auto max-w-7xl px-6 lg:px-8">
        <div class="mx-auto max-w-3xl text-center">
          <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">Applications</h2>
          <p class="mt-2 text-lg leading-8 text-gray-600">
            <br>
            <b>
            Kaolin, as a versatile mineral, finds extensive applications in the ceramic industry.

            </b>
<br>
<br>
For ceramic manufacturers, it serves as a fundamental raw material for producing high-quality and durable ceramics. In the realm of glaze and pigment industries, Kaolin enhances the properties of colors and glazes.
<br>
<br>
Beyond ceramics, Kaolin serves diverse purposes in several industries. Its applications span the production of cosmetics, pharmaceuticals, and paper, showcasing its versatility as a valuable mineral with unique properties.

          </p>
        </div>
        <div class="mx-auto mt-16 grid max-w-2xl auto-rows-fr grid-cols-1 gap-8 sm:mt-20 lg:mx-0 lg:max-w-none lg:grid-cols-3">
          <article v-for="post in posts" :key="post.id" class="relative isolate flex flex-col justify-end overflow-hidden rounded-2xl bg-gray-900 px-8 pb-8 pt-80 sm:pt-48 lg:pt-80">
            <img :src="post.imageUrl" alt="" class="absolute inset-0 -z-10 h-full w-full object-cover" />
            <div class="absolute inset-0 -z-10 bg-gradient-to-t from-gray-900 via-gray-900/40" />
            <div class="absolute inset-0 -z-10 rounded-2xl ring-1 ring-inset ring-gray-900/10" />
  
            <div class="flex flex-wrap items-center gap-y-1 overflow-hidden text-sm leading-6 text-gray-300">
              <div class="-ml-4 flex items-center gap-x-4">
                <svg viewBox="0 0 2 2" class="-ml-0.5 h-0.5 w-0.5 flex-none fill-white/50">
                  <circle cx="1" cy="1" r="1" />
                </svg>
             
              </div>
            </div>
            <h3 class="mt-3 text-lg font-semibold leading-6 text-white">
              <div>
                <span class="absolute inset-0" />
                {{ post.title }}
              </div>
            </h3>
          </article>
        </div>
      </div>
    </div>
  </template>
  
  <script setup>
  const posts = [
    {
      id: 1,
      title: 'ceramic',
  
    imageUrl:
        '/photo/6.jpg',
  

    },
    {
      id: 1,
      title: 'ceramic tile',
  
    imageUrl:
        '/photo/5.jpg',
  

    },
    {
      id: 1,
      title: 'Engineered Stone',
  
    imageUrl:
        '/photo/7.jpg',
  

    },
    // More posts...
  ]
  </script>