<script setup>
const {data} = await useFetch('/api/example',{
    method: 'post',
    body:{ name:'Alex', id: 1 }
})
</script>

<template>
    <div>
        <h1>Home page</h1>
    </div>
    <Alert color="primary">
        {{ data.mess }}
    </Alert>
</template>

<style scoped>
    h1{
        color:red
    }
</style>