<template>
    <Navbar />
    <main class="d-flex">
        <section class="col-4">
            <EntryList />
        </section>
        <section class="col p-relative">
            <router-view />
        </section>
    </main>
</template>

<script>
import { defineAsyncComponent } from 'vue';

export default {
    components: {
        Navbar: defineAsyncComponent(() => import('../components/Navbar.vue')),
        EntryList: defineAsyncComponent(() => import('../components/EntryList.vue')),
    }
}
</script>