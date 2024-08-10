<script lang="ts">
    import type { Work } from "../../types/Work";
    export let job:Work;
    const dateOptions: Intl.DateTimeFormatOptions = { year: 'numeric', month: 'long' };
</script>

<div class="bg-gradient-to-tr from-slate-900 to-slate-800 rounded-xl overflow-hidden shadow-md p-6">
  <h3 class="text-2xl font-semibold text-white mb-2">{job.role}</h3>
  <h4 class="text-xl text-sky-400 mb-3">{job.organization}</h4>
  <p class="text-slate-100 mb-4">{job.startDate.toLocaleString('default', dateOptions)} - {job.endDate.toLocaleString('default', dateOptions)}</p>
  <ul class="text-slate-100 list-disc list-inside space-y-2">
  {#each job.contribution as contribution}
    <li>{contribution}</li>
  {/each}
  </ul>
</div>