<script lang="ts">
  import type { Snippet } from "svelte";

  const { stat, description }: { stat: Snippet; description: Snippet } =
    $props();
</script>

<div class="flex flex-col gap-3 border border-primary p-3 aspect-square font-light">
  <h1 class="text-6xl text-left">
    {@render stat()}
  </h1>
  <div class="text-left text-2xl">
    {@render description()}
  </div>
</div>
