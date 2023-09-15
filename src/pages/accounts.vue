<template>
  <div class="m-4">
    <RouterLink to="/about">Import account</RouterLink>
    <h1>List Accounts</h1>
    <button @click="$router.back">Go Back</button>
  </div>
</template>

<script>
export default {
  name: "Accounts"
}
</script>

<style scoped>

</style>
