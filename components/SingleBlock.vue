<template>
  <div class="grid grid-col-12">
    <div class="col-span-12">
      <div class="flex flex-col justify-center items-center border-2 border-red-500 my-2">
        <div class="text-center">
          <ContentDoc path="/single" v-slot="{ doc }">
            <h2 class="text-center">{{ doc.title }}</h2>
            <p>
              <ContentRenderer :value="doc" />
            </p>
            <div class="text-center">
              <button class="text-cetner">{{ doc.button }}</button>
            </div>
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
