<script setup lang="ts">
    import 'remixicon/fonts/remixicon.css';
</script>

<template>
    <section id="search-form">
        <form action="https://www.google.com/search" target="_blank">
            <input type="text" name="q" ref="query" placeholder="Type any keyword to search on internet">
            <button type="submit">
                <i class="ri-search-line"></i>
            </button>
        </form>
    </section>
</template>

<style scoped>

</style>