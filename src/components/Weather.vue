<script setup lang="ts">
    import { ref, Ref } from 'vue';

    const weatherContent: Ref = ref(null);

    fetch(`https://wttr.in`)
        .then((r: any) => r.text())
        .then((d: any) => {
            weatherContent.value = d.replaceAll(/.*<a[^>]+>[^<]+<\/a>.*/ig, '');
        });
</script>

<template>
    <section id="weather" v-html="weatherContent">
    </section>
</template>

<style scoped>

</style>