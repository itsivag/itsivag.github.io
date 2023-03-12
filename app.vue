<script>
export default {
  methods: {
    sendEmail() {
      const email = "sivacbrf2@gmail.com";
      const subject = "Your Portfolio is Lit!";
      const body = "Hello Siva, I'm reaching out from your portfolio!";
      const mailtoUrl = `mailto:${email}?subject=${encodeURIComponent(subject)}&body=${encodeURIComponent(body)}`;
      window.open(mailtoUrl);
    }
  }
}
</script>

<template>
  <div class="font-['Abel'] bg-neutral-800 text-white flex flex-row">
    <nav class=" bg-stone-900 p-4 h-screen flex flex-col max-w-[25vw]">
      <div class="px-2 hover:text-yellow-500">itsivag</div>
      <ul class="text-white h-full flex flex-col justify-center">
        <li
          class="px-1 hover:text-yellow-500 hover:border hover:py-7 hover:text-2xl hover:font-extrabold border-yellow-500">
          <NuxtLink to="/">Home</NuxtLink>
        </li>
        <li
          class="px-1 hover:text-yellow-500 hover:border hover:py-7 hover:text-2xl hover:font-extrabold border-yellow-500">
          <NuxtLink to="/about">About</NuxtLink>
        </li>
        <li
          class="px-1 hover:text-yellow-500 hover:border hover:py-7 hover:text-2xl hover:font-extrabold border-yellow-500">
          <NuxtLink to="/projects">Projects</NuxtLink>
        </li>
      </ul>
      <div class="px-2">
        <button class="px-2 py-1 border border-yellow-500 hover:bg-yellow-500" @click="sendEmail"> 
          Let's talk
        </button>
      </div>
    </nav>
    <NuxtPage />
  </div>
</template>
