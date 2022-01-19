<template>
  <div class="flex flex-col h-screen">
    <header class="relative px-5 text-red h-80 bg-purple-900">
      <h1 class="absolute text-7xl text-white" style="bottom:-9px;">2022</h1>
    </header>
    <main class="grow p-5">
      <router-view />
    </main>
    <footer class="border px-5 py-2">
      <ul class="flex justify-end">
        <li class="mr-3">Quarter Begins</li>
        <li class="mr-3">Quarter Ends</li>
        <li class="mr-3">Holiday</li>
      </ul>
    </footer>
  </div>
</template>

<script>
export default {
  name: "App",
  components: {
  },
};
</script>
