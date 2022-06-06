<template>
  <article class="entry-container mb-3 pointer p-2" @click="$router.push({ name: 'entry', params: { id: 10 } })" >
    <div class="entry-title d-flex">
      <span class="text-success fs-5 fw-bold">31</span>
      <span class="mx-1 fs-5">Mayo</span>
      <span class="mx-1 fs-5">2022</span>
    </div>

    <div class="entry-description">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Excepturi
      praesentium facere esse reprehenderit neque vitae expedita iusto, dolorem
      ea minus.
    </div>
  </article>
</template>

<style lang="scss" scoped>
.entry-container {
    border-bottom: 1px solid #2c3e50;
    transition: 200ms all ease-in;

    &:hover {
        background-color: lighten($color: grey, $amount: 45);
        transition: 200ms all ease-in;
    }

    .entry-description {
        font-size: 14px;
    }
}
</style>