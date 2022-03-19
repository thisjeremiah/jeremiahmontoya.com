<script lang="typescript">
  export let name: string
  export let role: string
  export let dates: string
  export let points = []
</script>

<div class="py-2">
  <div class="flex justify-between pb-1 font-serif">
    <h4 class="">{name}</h4>
    <h4 class="">{dates}</h4>
  </div>
  {#if role}
    <h5 class="text-sm">{role}</h5>
  {/if}
  <ul class="pl-4 list-disc">
    {#each points as point}
      <li class="pl-2 text-sm">{point}</li>
    {/each}
  </ul>
</div>
