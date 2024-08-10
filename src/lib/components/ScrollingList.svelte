<script>
  export let items;
  // Duplicate the list to create a seamless loop
  $: duplicatedItems = [...items, ...items];
</script>

<div class="overflow-hidden relative w-full" style="height: 3rem;">
  <div class="animate-scroll absolute left-0 flex whitespace-nowrap">
    {#each duplicatedItems as item}
      <div class="px-4 text-base sm:text-lg md:text-xl font-bold text-slate-200">{item}</div>
    {/each}
  </div>
</div>

<style>
  @keyframes scroll {
    0% {
      transform: translateX(0);
    }
    100% {
      transform: translateX(-50%);
    }
  }

  .animate-scroll {
    animation: scroll 60s linear infinite;
  }

  @media (max-width: 640px) {
    .animate-scroll {
      animation-duration: 30s;
    }
  }
</style>