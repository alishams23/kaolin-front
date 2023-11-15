<template>
    <div class="relative isolate overflow-hidden bg-gray-900 py-24 sm:py-32">
        <div class="mx-auto max-w-7xl px-6 lg:px-8">
          <div class="mx-auto max-w-2xl lg:max-w-none">
            <div class="text-center">
              <h2 class="text-3xl font-bold tracking-tight text-white sm:text-4xl">
                Trusted by industrial companies worldwide</h2>
              <p class="mt-4 text-lg leading-8 text-gray-300">We invite you to use our products.</p>
            </div>
            <dl class="mt-16 grid grid-cols-1 gap-0.5 overflow-hidden rounded-2xl text-center sm:grid-cols-2 lg:grid-cols-4">
              <div v-for="stat in stats" :key="stat.id" class="flex flex-col bg-white/5 p-8">
                <dt class="text-sm font-semibold leading-6 text-gray-300">{{ stat.name }}</dt>
                <dd class="order-first text-3xl font-semibold tracking-tight text-white">{{ stat.value }}</dd>
              </div>
            </dl>
          </div>
        </div>
        <svg class="absolute inset-0 h-full w-full stroke-gray-700 [mask-image:radial-gradient(100%_100%_at_top_left,white,transparent)]" aria-hidden="true">
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
</template>
<script setup>
const stats = [
  { id: 1, name: 'Employees', value: '2,000+' },
  { id: 2, name: 'Countries', value: '21' },
  { id: 3, name: 'Technical centres', value: '3' },
  { id: 4, name: 'Customers', value: '500+' },
]
</script>