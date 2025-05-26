<script>
  import Nav from "$lib/nav.svelte";
  let { children } = $props();
</script>

<Nav />

{@render children()}
