<template>
    <div>
        <image src="" width="100px" style="aspect-ratio: 1 / 1;" />
        <p>{{ album }} ({{ year }}) - {{ artist }}</p>
    </div>
</template>

<script>
    export let album = '';
    export let year = '';
    export let artist = '';
</script>