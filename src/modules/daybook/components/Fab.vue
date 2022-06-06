<template>
  <button type="button" class="btn btn-dark">
    <em :class="`fa fa-2x ${this.icon}`"></em>
  </button>
</template>

<script>
export default {
  props: {
    icon: {
      type: String,
      default: 'fa-plus'
    }
  }
}
</script>

<style lang="scss" scoped>
button {
  border-radius: 100%;
  bottom: 10px;
  height: 60px;
  position: fixed;
  right: 10px;
  width: 60px;
}
</style>