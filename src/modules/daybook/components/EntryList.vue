<template>
  <article class="entry-list-container px-2">
    <div class="py-2 w-md-50">
      <input
        type="text"
        name="search"
        id="search"
        placeholder="Buscar entrada"
        class="form-control"
      />
    </div>
    <div class="entry-scrollarea">
      <Entry v-for="item in 100" :key="item" />
    </div>
  </article>
</template>

<script>
import { defineAsyncComponent } from "@vue/runtime-core";
export default {
  name: "EntryList",
  components: {
    Entry: defineAsyncComponent(() => import("./Entry.vue")),
  },
};
</script>

<style lang="scss" scoped>
.entry-list-container {
  border-right: 0.5px solid #2c3e50;
  height: calc(100vh - 63px);
}
.entry-scrollarea {
  overflow-y: auto;
  height: calc(100% - 70px);
}
</style>
