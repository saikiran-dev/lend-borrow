<template>
  <div class="w-1/4 max-w-xs bg-zinc-800 min-h-full">
    <p class="text-2xl tracking-wide text-center text-emerald-300">
      Lend & Borrow
    </p>
    <Nav />
  </div>
</template>
<script>
import Nav from "./Nav.vue";
export default {
  name: "Sidebar",
  components: {
    Nav,
  },
};
</script>
