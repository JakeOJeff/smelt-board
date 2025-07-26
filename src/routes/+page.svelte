<script lang="ts">
    type Item = { id: number; content: null;};
    let items: Item[] = [];
</script>
<h1 class="text-3xl font-bold underline">
  Hello world!
</h1>
<div>
    {#each items as item (item.id)}
    <div>
        {item.content}
        </div>
        {/each}
</div>

<style lang="postcss">
  @reference "tailwindcss";
  :global(html) {
    background-color: theme(--color-gray-100);
  }
</style>