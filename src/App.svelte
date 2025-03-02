<script lang="ts">
  import Stat from "./Stat.svelte";
</script>

<main class="flex">
  <div class="flex flex-col gap-8 m-auto max-w-[600px] text-center">
    <h1 class="text-6xl">
      {import.meta.env.VITE_TARGET_NAME}'s Sleep Loss Tracker
    </h1>

    <div class="flex gap-8">
      <Stat>
        {#snippet stat()}
          25
        {/snippet}
        {#snippet description()}
          hours of sleep lost.
        {/snippet}
      </Stat>
      <Stat>
        {#snippet stat()}
          400
        {/snippet}
        {#snippet description()}
          braincells missing.
        {/snippet}
      </Stat>
    </div>
  </div>
</main>
