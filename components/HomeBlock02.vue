<template>
  <div class="grid grid-col-12">
    <div class="col-span-12">
      <div class="flex flex-col justify-center items-center border-2 border-red-500 my-2">
        <ContentDoc path="/home/block02" v-slot="{ doc }">
          <h1 class="text-center">{{ doc.title }}</h1>
          <p class="py-6"><ContentRenderer :value="doc" /></p>
          <button class="mx-auto">
            {{ doc.button }}
          </button>
        </ContentDoc>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
div {
  content: "";
}
</style>
