<template>
  <div class="flex flex-col h-screen">
    <header class="relative px-5 text-red bg-purple-900" style="height:170px;">
      this is the header
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
