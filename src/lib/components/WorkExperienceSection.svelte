<script lang='ts'>
  import WorkCard from "./WorkCard.svelte";
  import type { Work } from "../../types/Work";
  
  const jobs:Work[] = [
    {
      role: 'Technology Intern',
      organization: 'HERD International',
      startDate: new Date(2024, 6, 3),
      endDate: new Date(2024, 8, 9),
      contribution: ['Contrib1', 'Contrib2']
    },
    {
      role: 'Website Dev & Intern',
      organization: 'Anweshan',
      startDate: new Date(2024, 6, 3),
      endDate: new Date(2024, 8, 9),
      contribution: ['Contrib1', 'Contrib2']
    }
  ]
</script>

<div id="experience" class="font-sans bg-gradient-to-br from-black to-slate-800 px-8 sm:px-24 md:px-36 pb-12">
  <h2 class="py-2 text-4xl sm:text-5xl font-bold text-white mb-12 text-center bg-gradient-to-r from-blue-50 to-blue-700 text-transparent bg-clip-text">Experience</h2>
  <div class="space-y-8">
    {#each jobs as job}
      <WorkCard job={job} />
    {/each}
  </div>
</div>
