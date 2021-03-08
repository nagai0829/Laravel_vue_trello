<template>
    <div class="container">
        <form
    class="relative mb-3 flex flex-col justify-between bg-white rounded-md shadow overflow-hidden"
    post="tasks"
  >
    <div class="p-3 flex-1">
      <input
        class="block w-full px-2 py-1 text-lg border-b border-blue-800 rounded"
        type="text"
        placeholder="Enter a title"
      />
      <textarea
        class="mt-3 p-2 block w-full p-1 border text-sm rounded"
        rows="2"
        placeholder="Add a description (optional)"
      ></textarea>
      <!-- <div v-show="errorMessage">
        <span class="text-xs text-red-500">
          {{ errorMessage }}
        </span>
      </div> -->
    </div>
    <div class="p-3 flex justify-between items-end text-sm bg-gray-100">
      <!-- <button
        @click="$emit('task-canceled')"
        type="reset"
        class="py-1 leading-5 text-gray-600 hover:text-gray-700"
      >
        キャンセル
      </button> -->
      <button
        type="submit"
        class="px-3 py-1 leading-5 text-white bg-orange-600 hover:bg-orange-500 rounded"
      >
        追加
      </button>
    </div>
  </form>
    </div>
</template>

<script>
    export default {
        mounted() {
            console.log('Component mounted.')
        }
    }
</script>
