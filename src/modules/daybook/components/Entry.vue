<template>
  <div class="entry-container mb-3 pointer p-2"
    @click="$router.push({name: 'entry', params: {id: 10} })"
        >
    <div class="entry-title d-flex">
        <span class="text-success fs-5 fw-bold">20</span>
        <span class="mx-2 fs-5">Enero</span>
        <span class="">2023, Viernes</span>
    </div>
    <div class="entry-description">
        Sunt dolore aliquip ea enim aliquip et do in esse fugiat cupidatat. Fugiat sunt dolore magna voluptate proident laborum duis reprehenderit irure pariatur aliquip aliquip id. Et ut pariatur aliquip quis. Ullamco eu ut qui do est incididunt.
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
    .entry-container {
        border-bottom: 1px solid #2c3e50;
        transition: 0.2s all ease-in;

        &:hover {
            background-color: lighten($color: grey, $amount: 45);
        }

        .entry-description {
            font-size: 12px;
        }
    }

</style>