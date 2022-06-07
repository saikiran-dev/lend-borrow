<template>
  <div class="dashboard flex min-h-screen w-full">
    <Sidebar />
    <ContentPage />
  </div>
</template>
<script>
// @ is an alias to /src
import ContentPage from "@/components/global/ContentPage.vue";
import Sidebar from "@/components/global/Sidebar.vue";

export default {
  name: "DashboardView",
  components: {
    ContentPage,
    Sidebar,
  },
};
</script>
