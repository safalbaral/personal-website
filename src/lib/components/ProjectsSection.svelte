<script>
  let projects = [
   {
     title: 'Koi Time',
     description: 'A brief description of project 1. Lorem Ipsum.',
     tags: ['React Native', 'SQLite', 'Redux', 'Mobile Development'],
     image: '/src/assets/images/KoiTime.png'
   },
   {
     title: 'HERD Project',
     description: 'A brief description of project 2. Lorem Ipsum.',
     tags: ['Tag', 'Tag'],
     image: '/src/assets/images/NepalDistricts.png'
   },
   {
     title: 'The Cocoon - An Environment Redesign Project',
     description: 'A brief description of project 3. Lorem Ipsum.',
     tags: ['Raspberry Pi Pico W', '3D Modelling & Printing', 'MicroPython', 'React', 'Microcontroller Development', 'Web Development'],
     image: '/src/assets/images/SUTD_DTI.png'
   },
   {
     title: 'Billing',
     description: 'A brief description of the project. Lorem Ipsum',
     tags: ['Python', 'Flask'],
     image: '/src/assets/images/BillGenerator.png'
   }
 ];
 </script>
 
 <div id="projects" class="font-sans bg-gradient-to-tr from-black to-slate-800 p-4 sm:p-8">
   <h2 class="py-2 text-3xl sm:text-4xl md:text-5xl font-bold text-white mb-8 sm:mb-12 text-center bg-gradient-to-r from-blue-200 to-blue-900 text-transparent bg-clip-text">Projects</h2>
   <div class="grid grid-cols-1 md:grid-cols-2 gap-6 sm:gap-8 px-2 sm:px-8 md:px-16">
     {#each projects as project}
       <div class="cursor-pointer bg-gradient-to-tr from-slate-900 to-slate-800 rounded-xl overflow-hidden shadow-md transition-all duration-300 hover:shadow-xl hover:-translate-y-2">
         <img src={project.image} alt={project.title} class="w-full h-48 sm:h-56 object-cover" />
         <div class="p-4 sm:p-6">
           <h3 class="text-xl sm:text-2xl font-semibold text-white mb-2 sm:mb-3">{project.title}</h3>
           <p class="text-slate-100 mb-3 sm:mb-4 text-sm sm:text-base line-clamp-3">{project.description}</p>
           <div class="flex flex-wrap gap-2 mt-auto">
             {#each project.tags as tag}
               <span class="bg-sky-100 text-sky-800 px-2 py-1 rounded-full text-xs sm:text-sm font-medium mb-1">
                 {tag}
               </span>
             {/each}
           </div>
         </div>
       </div>
     {/each}
   </div>
 </div>