<script lang="ts">
    import "../css/app.css";
    import favicon from "$lib/assets/favicon.svg";
    import Fade from "$lib/components/Fade.svelte";
    let { children } = $props();
</script>

<svelte:head>
    <link rel="icon" href={favicon} />
</svelte:head>

<main class="flex flex-col">
    {@render children?.()}
</main>
