<template>
  <div class="grid grid-col-12">
    <div class="col-span-12">
      <div class="flex flex-col justify-center items-center border-2 border-red-500 my-2">
        <div>
          <ContentDoc path="/main/banner" v-slot="{ doc }">
            <h1 class="text-center">{{ doc.title }}</h1>
            <small>{{ doc.description }}</small>
            <p class="text-center">
              <ContentRenderer :value="doc" />
            </p>
            <button class="text-center">{{ doc.button }}</button>
          </ContentDoc>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
main {
  border: 1px solid green;

  h1:nth-child(3) {
    background: green;
  }
}
</style>
