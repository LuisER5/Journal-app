<template>
    <article class="d-flex justify-content-center h-100">
        <h1 class="align-self-center">No hay nada seleccionado</h1>
        <Fab />
    </article>
</template>

<script>
import { defineAsyncComponent } from '@vue/runtime-core'
export default {
    components: {
        Fab: defineAsyncComponent(() => import('../components/Fab.vue'))
    }
}
</script>