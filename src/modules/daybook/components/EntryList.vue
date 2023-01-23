<template>
    <div class="entry-list-container">
        <div class="px-2 pt-2">
            <input type="text" class="form-control" placeholder="Buscar Entrada">
        </div>
    </div>
    <div class="entry-scrollarea">
        <Entry v-for="item in 100" :key="item" />
    </div>
</template>

<script>
import { defineAsyncComponent } from 'vue'

export default {
    components: {
        Entry: defineAsyncComponent(() => import('./Entry.vue'))
    }
}
</script>

<style lang="scss" scoped>
    input {
        height: 25px;
    }
    .entry-list-container {
        border-right: 1px solid #2c3e50;
        height: calc(100vh - 670px);
    }
    .entry-scrollarea {
        height: calc(100vh - 135px);
        overflow: scroll;
    }
</style>