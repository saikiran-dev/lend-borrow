<template>
  <div>
    <div class="grid grid-cols-2 gap-2">
      <div>
        <label
          for="transaction-with"
          class="block text-sm font-medium text-gray-700"
          >Transaction With</label
        >
        <input
          type="text"
          name="transaction-with"
          id="transaction-with"
          class="p-2 border mt-1 block shadow-sm border-gray-300 rounded-md"
        />
      </div>
      <div>
        <label
          for="transaction-type"
          class="block text-sm font-medium text-gray-700"
          >Transaction Type</label
        >
        <input
          type="text"
          name="transaction-type"
          id="transaction-type"
          class="p-2 border mt-1 block shadow-sm border-gray-300 rounded-md"
        />
      </div>
      <div>
        <label
          for="transaction-date"
          class="block text-sm font-medium text-gray-700"
          >Transaction Date</label
        >
        <input
          type="text"
          name="transaction-date"
          id="transaction-date"
          class="p-2 border mt-1 block shadow-sm border-gray-300 rounded-md"
        />
      </div>
      <div>
        <label
          for="transaction-date"
          class="block text-sm font-medium text-gray-700"
          >Transaction Date</label
        >
        <Datepicker
          placeholder="Select Date"
          v-model="customDate"
          format="dd-MM-yyyy"
        ></Datepicker>
      </div>
      <div>
        <label for="reason" class="block text-sm font-medium text-gray-700">
          Reason
        </label>
        <div class="mt-1">
          <textarea
            id="reason"
            name="reason"
            rows="3"
            class="p-2 shadow-sm mt-1 block w-full sm:text-sm border border-gray-300 rounded-md"
          ></textarea>
        </div>
      </div>
      <div></div>
    </div>
  </div>
</template>
<script>
import Datepicker from "vuejs-datepicker";
export default {
  name: "AddExpenseForm",
  components: {
    Datepicker,
  },
  data() {
    return {
      customDate: null,
    };
  },
};
</script>
<style>
.vdp-datepicker,
.vdp-datepicker div > input {
  /* border: 1px solid black; */
  border-radius: 0.375rem;
}
.vdp-datepicker div > input {
  border: 1px solid black;
  padding: 4px;
}
</style>
