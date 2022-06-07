<template>
  <div
    class="relative z-10"
    aria-labelledby="modal-title"
    role="dialog"
    aria-modal="true"
  >
    <div
      class="fixed inset-0 bg-gray-500 bg-opacity-75 transition-opacity"
    ></div>

    <div class="fixed z-10 inset-0 overflow-y-auto">
      <div
        class="flex items-end sm:items-center justify-center min-h-full p-4 text-center sm:p-0"
      >
        <div
          class="relative bg-white rounded-lg text-left overflow-hidden shadow-xl transform transition-all sm:my-8 sm:max-w-lg sm:w-full"
        >
          <div class="bg-white px-4 pt-5 pb-4 sm:p-6 sm:pb-4">
            <AddExpense />
            <div class="px-4 py-3 text-right sm:px-6">
              <button
                type="submit"
                class="inline-flex justify-center py-2 px-4 border shadow-sm text-sm font-medium rounded-md text-black hover:bg-gray-200 mr-4"
                @click="closeModal"
              >
                Cancel
              </button>
              <button
                type="submit"
                class="inline-flex justify-center py-2 px-4 border border-transparent shadow-sm text-sm font-medium rounded-md text-white bg-indigo-600 hover:bg-indigo-700"
                @click="saveData"
              >
                Save
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import AddExpense from "@/components/forms/AddExpenseForm.vue";
export default {
  name: "Modal",
  props: ["closeModal", "saveData"],
  components: {
    AddExpense,
  },
};
</script>
