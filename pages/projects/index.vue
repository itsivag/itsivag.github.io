<template>
  <div class="h-screen w-[80vw]">
    <h1 class="py-8 px-4 text-3xl">
      Behold, My <span class="text-yellow-500">Epic Projects</span> :
    </h1>

    <div class="flex p-4">
      <NuxtLink to="projects/dlapp"
        class="flex  flex-1 flex-col m-2 p-4 border border-white hover:border-yellow-500  hover:pb-28 hover:pr-32  hover:bg-stone-900 hover:text-white">
        <h1 class="text-2xl font-medium text-yellow-500 hover:underline">DLAAP :</h1>
        <br>
        <p class="text-xl">
          DLAPP is a mobile app that enables staff members of Anna University regional campus Coimbatore to request and
          approve permissions with ease and efficiency.
        </p>
        <div class="px-1 pt-4 pb-2">
          <span
            class="hover:bg-yellow-500 hover:text-gray-100 inline-block bg-gray-200 px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#android</span>
          <span
            class="hover:bg-yellow-500 hover:text-gray-100 inline-block bg-gray-200 px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#firebase</span>
        </div>
      </NuxtLink>

      <NuxtLink class="flex flex-1 flex-col border border-white m-2 p-4 hover:border-yellow-500 hover:pb-28 hover:pr-32 hover:bg-stone-900  hover:text-white " 
        to="projects/Wallbyte">
        <h1 class="text-2xl font-medium text-yellow-500 hover:underline">Wallbyte :</h1>
        <br>
        <p class="text-xl">
          A Firebase-powered Android app that lets you browse and set beautiful wallpapers with ease and efficiency.
        </p>
        <div class="px-1 pt-4 pb-2">
          <span
            class="hover:bg-yellow-500 hover:text-gray-100 inline-block bg-gray-200 px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#kotlin</span>
          <span
            class="hover:bg-yellow-500 hover:text-gray-100 inline-block bg-gray-200 px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#xml</span>
          <span
            class="hover:bg-yellow-500 hover:text-gray-100 inline-block bg-gray-200 px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#glide</span>
        </div>
      </NuxtLink>
    </div>

    <div class="flex p-4">
      <NuxtLink to="projects/dlapp"
        class="flex  flex-1 flex-col m-2 p-4 border border-white hover:border-yellow-500  hover:pb-28 hover:pr-32   hover:bg-stone-900">
        <h1 class="text-2xl font-medium text-yellow-500 hover:underline">DLAAP :</h1>
        <br>
        <p class="text-xl">
          DLAPP is a mobile app that enables staff members of Anna University regional campus Coimbatore to request and
          approve permissions with ease and efficiency.
        </p>
        <div class="px-1 pt-4 pb-2">
          <span
            class="hover:bg-yellow-500 hover:text-gray-100 inline-block bg-gray-200 px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#android</span>
          <span
            class="hover:bg-yellow-500 hover:text-gray-100 inline-block bg-gray-200 px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#firebase</span>
        </div>
      </NuxtLink>

      <NuxtLink class="flex flex-1 flex-col border border-white m-2 p-4 hover:border-yellow-500 hover:pb-28 hover:pr-32   hover:bg-stone-900"
        to="projects/Wallbyte">
        <h1 class="text-2xl font-medium text-yellow-500 hover:underline">Wallbyte :</h1>
        <br>
        <p class="text-xl">
          A Firebase-powered Android app that lets you browse and set beautiful wallpapers with ease and efficiency.
        </p>
        <div class="px-1 pt-4 pb-2">
          <span
            class="hover:bg-yellow-500 hover:text-gray-100 inline-block bg-gray-200 px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#kotlin</span>
          <span
            class="hover:bg-yellow-500 hover:text-gray-100 inline-block bg-gray-200 px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#xml</span>
          <span
            class="hover:bg-yellow-500 hover:text-gray-100 inline-block bg-gray-200 px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#glide</span>
        </div>
      </NuxtLink>
    </div>
  </div>
</template>
