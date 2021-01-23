<template>
  <div
    class="flex flex-col justify-between lg:w-2/4 h-32 border rounded-sm mb-5 mx-auto bg-white"
  >
    <div class="h-6 text-gray-700 px-1 text-right">
      <span class="text-xs text-gray-500 font-medium">{{ comment.date }}</span>
      <div class="border-b w-11/12 mx-auto border-green-600 pb-2"></div>
    </div>
    <div class="px-2">
      <div>
        <p class="font-light text-sm text-gray-600">{{ comment.message }}</p>
      </div>
    </div>
    <div
      class="flex flex-row justify-between px-2 text-xs bg-green-200 text-gray-700"
    >
      <span class="font-semibold">{{ comment.author }}</span>
      <div>
        <span>likes: {{ comment.likes }}</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ['comment'],
}
</script>
