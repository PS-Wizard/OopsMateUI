<script>
    import { fade } from "svelte/transition";

    let {children} = $props()
</script>

<div in:fade={{delay:250, duration:250}} out:fade={{duration:250}}>
    {@render children()}
</div>
