<template>
  <div class="text-center p-6 rounded-lg bg-zinc-900 mr-6">
    <p>{{ title }}</p>
    <p
      class="flex items-center"
      :class="[owe ? 'text-red-500' : 'text-green-500']"
    >
      <RupeeIcon classes="h-5 w-5" :color="[owe ? '#ef4444' : '#22c55e']" />
      <span class="text-2xl">{{ amount }}</span>
    </p>
  </div>
</template>
<script>
import RupeeIcon from "@/assets/svgs/rupee-svg.vue";
export default {
  name: "BalanceInfoCard",
  props: {
    title: {
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
    RupeeIcon,
  },
};
</script>
