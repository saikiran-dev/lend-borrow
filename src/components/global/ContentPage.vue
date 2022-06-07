<template>
  <div class="content-page p-4 bg-black min-h-full w-full">
    <div class="flex justify-between max-w-lg">
      <button
        type="button"
        class="text-white py-4 px-6 bg-emerald-600 rounded-lg"
        @click="enable = true"
      >
        Add expense
      </button>
      <button
        type="button"
        class="text-white py-4 px-6 bg-orange-600 rounded-lg"
      >
        Settle up
      </button>
    </div>

    <div class="balance-info-cards my-6 flex text-gray-500">
      <BalanceInfoCard title="Total Balance" amount="182.00" />
      <BalanceInfoCard :owe="true" title="You owe" amount="182.00" />
      <BalanceInfoCard title="You are owed" amount="182.00" />
    </div>
    <div class="flex max-w-7xl">
      <div class="balance-info-cards text-white mr-8 flex w-3/4">
        <OweList />
      </div>
      <ActivityList />
    </div>
    <Modal v-if="enable" :closeModal="closeModal" :saveData="saveData" />
  </div>
</template>
<script>
import BalanceInfoCard from "@/components/cards/BalanceInfoCard.vue";
import OweList from "@/components/lists/OweList.vue";
import ActivityList from "@/components/lists/ActivityList.vue";
import Modal from "@/components/Modal.vue";
export default {
  name: "ContentPage",
  components: {
    BalanceInfoCard,
    OweList,
    ActivityList,
    Modal,
  },
  data() {
    return {
      enable: false,
    };
  },
  methods: {
    closeModal() {
      this.enable = false;
    },
    saveData() {
      console.log("this is saved");
      this.closeModal();
    },
  },
};
</script>
