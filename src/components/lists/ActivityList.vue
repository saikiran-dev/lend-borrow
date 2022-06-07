<template>
  <div class="text-white w-full bg-zinc-900 rounded-lg max-w-lg">
    <p class="p-4 bg-zinc-800 rounded-lg">Recent Activity</p>
    <ActivityCard />
  </div>
</template>
<script>
import ActivityCard from "@/components/cards/ActivityCard.vue";
export default {
  name: "ActivityList",
  components: {
    ActivityCard,
  },
};
</script>
