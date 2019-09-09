<template>
    <div class="main-container">
        <Navbar/>
        <router-view/>

    </div>
</template>

<script>
    import Navbar from "../components/Navbar";
    export default {
        name: "mainLayout",
        components: {Navbar}
    }
</script>

<style scoped>

</style>
