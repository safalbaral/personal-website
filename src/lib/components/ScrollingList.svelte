<script>
    export let items;
  
    // Duplicate the list to create a seamless loop
    items = [...items, ...items];
  </script>
  <div class="overflow-hidden h-full relative">
    <div class="animate-scroll absolute left-0 flex">
      {#each items as item}
        <div class="px-4 whitespace-nowrap text-xl font-bold text-slate-200">{item}</div>
      {/each}
    </div>
  </div>
  
  <style>
    @keyframes scroll {
      0% {
        transform: translateX(0);
      }
      100% {
        transform: translateX(-30%);
      }
    }
  
    .animate-scroll {
      animation: scroll 60s linear infinite;
    }
  </style>