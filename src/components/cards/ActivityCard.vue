<template>
  <div class="flex items-center">
    <CheckIcon />
    <div class="text-gray-400">
      <p>You added "Demo"</p>
      <p class="text-gray-500 text-xs flex items-center">
        you get <RupeeIcon color="#22c55e" />
        <span :class="[owe ? 'text-red-500' : 'text-green-500']"> 52.61</span>
      </p>
      <p class="text-gray-500 text-xs">Today</p>
    </div>
  </div>
</template>
<script>
import CheckIcon from "@/assets/svgs/checklist.vue";
import RupeeIcon from "@/assets/svgs/rupee-svg.vue";
export default {
  name: "ActivityCard",
  props: {
    // name: {
    //   type: String,
    //   required: true,
    // },
    // amount: {
    //   required: true,
    // },
    owe: {
      default: false,
    },
  },
  components: {
    CheckIcon,
    RupeeIcon,
  },
};
</script>
