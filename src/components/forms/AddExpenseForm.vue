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
          class="px-2 border mt-1 block shadow-sm border-gray-300 rounded-md"
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
          class="px-2 border mt-1 block shadow-sm border-gray-300 rounded-md"
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
          class="px-2 border mt-1 block shadow-sm border-gray-300 rounded-md"
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
          class="px-2 border mt-1 block shadow-sm border-gray-300 rounded-md"
        />
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
            class="shadow-sm mt-1 block w-full sm:text-sm border border-gray-300 rounded-md"
          ></textarea>
        </div>
      </div>
    </div>
  </div>
</template>
