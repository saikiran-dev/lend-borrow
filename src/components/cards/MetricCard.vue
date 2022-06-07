<template>
  <div class="flex items-center">
    <UserIcon />
    <div>
      <p class="text-gray-400">{{ name }}</p>
      <div class="flex items-center">
        <span class="text-xs text-gray-500 mr-1">you owe</span>
        <RupeeIcon :color="[owe ? '#ef4444' : '#22c55e']" />
        <span
          class="text-xs"
          :class="[owe ? 'text-red-500' : 'text-green-500']"
        >
          {{ amount }}</span
        >
      </div>
    </div>
  </div>
</template>
<script>
import UserIcon from "@/assets/svgs/user-svg.vue";
import RupeeIcon from "@/assets/svgs/rupee-svg.vue";
export default {
  name: "MetricCard",
  props: {
    name: {
      type: String,
      required: true,
    },
    amount: {
      required: true,
    },
    owe: {
      default: false,
    },
  },
  components: {
    UserIcon,
    RupeeIcon,
  },
};
</script>
