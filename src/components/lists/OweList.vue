<template>
  <div class="flex">
    <!-- ------youOweList-------- -->
    <div class="you-owe-list rounded-lg bg-zinc-900 w-1/2">
      <p class="p-4 rounded-tl-lg rounded-bl-lg bg-zinc-800">YOU OWE</p>
      <div v-for="item in youOweList" :key="item.name" class="mb-4">
        <MetricCard :owe="true" :name="item.name" :amount="item.amount" />
      </div>
    </div>
    <!-- ------youAreOwedList-------- -->
    <div class="you-are-owed-list rounded-lg bg-zinc-900 w-1/2">
      <p class="p-4 rounded-tr-lg rounded-br-lg bg-zinc-800">YOU ARE OWED</p>
      <div v-for="(item, index) in youAreOwedList" :key="index">
        <MetricCard :name="item.name" :amount="item.amount" />
      </div>
    </div>
  </div>
</template>
<script>
import MetricCard from "@/components/cards/MetricCard.vue";
import { youOwe, youAreOwed } from "../static/owe";
export default {
  name: "OweList",
  components: {
    MetricCard,
  },
  computed: {
    youOweList() {
      return youOwe;
    },
    youAreOwedList() {
      return youAreOwed;
    },
  },
};
</script>
<style type="text/css" scoped>
.you-owe-list,
.you-are-owed-list {
  min-width: 240px;
}
</style>
