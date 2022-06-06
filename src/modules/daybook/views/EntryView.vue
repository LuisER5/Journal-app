<template>
  <article>
    <div class="entry-title d-flex justify-content-between p-2">
      <div>
        <span class="text-success fs-3 fw-bold">31</span>
        <span class="mx-1 fs-3">Mayo</span>
        <span class="mx-2 fs-4">2022</span>
      </div>

      <div>
        <button type="button" class="btn btn-danger mx-2">
          Borrar
          <em class="fa fa-trash-alt"></em>
        </button>
        <button type="button" class="btn btn-success">
          Subir foto
          <em class="fa fa-upload"></em>
        </button>
      </div>
    </div>

    <hr />

    <article class="d-flex flex-column px-3 h-75">
      <textarea
        placeholder="¿Qué sucedió hoy?"
        name="description"
        id="description"
        cols="30"
        rows="10"
      ></textarea>
    </article>

    <Fab icon="fa-save" />

    <img
      class="img-thumbnail"
      src="https://i.redd.it/jeuusd992wd41.jpg"
      alt="pato"
    />
  </article>
</template>

<script>
import { defineAsyncComponent } from "@vue/runtime-core";
export default {
  name: "EntryView",

  components: {
    Fab: defineAsyncComponent(() => import("../components/Fab.vue")),
  },
};
</script>

<style lang="scss" scoped>
textarea {
  border: none;
  font-size: 20px;
  height: 100%;
  resize: none;

  &:focus {
    outline: none;
  }
}

img {
  bottom: 30px;
  left: 0;
  margin: auto;
  position: absolute;
  right: 0;
  width: 200px;
}
</style>
