<template>
    <div class="container">
        <h2>Child Component</h2>
        <p>{{ greeting }}</p>
    </div>
</template>
<script>
    export default {
        name: 'ProductComp',
        props: ['greeting'],
        components: {
        }
    }
</script>
<!-- Local styling if you make use of scoped -->
<style scoped>
.container {
    background-color: darkgreen;
    color: white;
}
</style>




