<template>
  <div class="grid grid-col-12">
    <div class="col-span-12">
      <div class="flex flex-col justify-center items-center border-2 border-red-500 my-2">
        <div class="text-center">
          <ContentDoc path="/about/block01" v-slot="{ doc }">
            <h2 class="text-center">{{ doc.title }}</h2>
            <p><ContentRenderer :value="doc" /></p>
          </ContentDoc>
        </div>
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
