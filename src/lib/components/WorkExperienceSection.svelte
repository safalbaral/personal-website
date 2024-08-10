<script lang='ts'>
  import WorkCard from "./WorkCard.svelte";
  import type { Work } from "../../types/Work";
  
  const jobs:Work[] = [
    {
      role: 'Technology Intern',
      organization: 'HERD International',
      startDate: new Date(2024, 5, 3),
      endDate: new Date(2024, 7, 9),
      contribution: ['Developed an interactive data visualization web application using React, Tailwind CSS, and Leaflet, enhancing data comprehension about the organization\'s projects.', 'Collaborated with a team to gather requirements and design a user-friendly interfaces, ensuring a smooth user experience.', 'Automated data processing by using Python to parse Excel files into JSON format, saving hours of time, which would otherwise have been required to convert the data.']
    },
    {
      role: 'Web Devloper Intern',
      organization: 'Anweshan',
      startDate: new Date(2023, 6, 10),
      endDate: new Date(2023, 8, 1),
      contribution: ['Collaborated with a team to redesign Anweshan\’s website, focusing on effectively communicating the organization\’s mission and research initiatives.', 'Developed the redesign using Wordpress as the CMS, and provided the team with a comprehensive explanations for content updates.', 'Gained valuable insights into project management and collaborative workflows within a research-focused environment.']
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
