<script>
  let { children, tile } = $props();
</script>

<details class="dropdown">
  <summary class="btn m-1">{tile}</summary>
  <ul
    class="menu dropdown-content bg-base-100 rounded-box z-1 w-52 p-2 shadow-sm"
  >
    {@render children()}
  </ul>
</details>
