<template>
    <div class="shortcutsContainer">
        <PageShortcut :title="'DuoLingo'" :color="'#aaaaaa'" />
        <PageShortcut :title="'GitHub'" :color="'#0b1114'"/>
        <PageShortcut :title="'Linkedin'" :color="'#196ec7'" />
    </div>
</template>

<script>

</script>

<style scoped>
    .shortcutsContainer {
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        max-width: 45vw;
        height: 230px;
        overflow: auto;
        justify-content: center;
    }

    ::-webkit-scrollbar {
        display: none;
    }
</style>