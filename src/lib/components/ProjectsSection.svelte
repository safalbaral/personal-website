<script>
  let projects = [
   {
     title: 'Koi Time',
     description: 'KoiTime is an Expo-powered React Native application that I started building for myself to help me track time spent on tasks and projects.',
     tags: ['React Native', 'Expo', 'SQLite', 'Redux', 'Mobile Development'],
     image: '/images/KoiTime.png',
     url: 'https://github.com/safalbaral/KoiTime'
   },
   {
     title: 'Nepal District Project Dashboard',
     description: 'This is an interactive dashboard I created at my internship, which my employer was kind enough to let me open source.',
     tags: ['React', 'TailwindCSS', 'LeafletJS', 'Data Visualization'],
     image: '/images/NepalDistricts.png',
     url: 'https://github.com/safalbaral/Nepal-Districts-Project-Map'
   },
   {
     title: 'The Cocoon - An Environment Redesign Project',
     description: 'Project created as part of SUTD\'s 3.007 course. Physical prototype with lights, sensors, and motors controlled with Raspberry Pi Pico W connected to an Adafruit backend, with commands sent through a React frontend.',
     tags: ['Raspberry Pi Pico W', '3D Modelling & Printing', 'MicroPython', 'React', 'Microcontroller Development', 'Web Development', 'IoT'],
     image: '/images/SUTD_DTI.png',
     url: 'https://github.com/safalbaral/TheCocoon-3.007_SUTD_DTI_Project'
   },
   {
     title: 'Flask PDF Invoices',
     description: 'A Flask web application I created for a family member to use for generating PDF invoices.',
     tags: ['Python', 'Flask', 'Bootstrap', 'Weasyprint', 'Web Development'],
     image: '/images/BillGenerator.png',
     url: 'https://github.com/safalbaral/Flask-PDF-Invoices'
   },
   {
     title: 'This Website',
     description: 'Designed using Svelte and TailwindCSS, made to be fully responsive on both desktop and mobile!',
     tags: ['Svelte', 'Typescript', 'TailwindCSS'],
     image: '/images/Website.png',
     url: 'https://github.com/safalbaral/personal-website'
   }
 ];
 </script>
 
 <div id="projects" class="font-sans bg-gradient-to-tr from-black to-slate-800 p-4 sm:p-8">
   <h2 class="py-2 text-3xl sm:text-4xl md:text-5xl font-bold text-white mb-8 sm:mb-12 text-center bg-gradient-to-r from-blue-200 to-blue-900 text-transparent bg-clip-text">Projects</h2>
   <p class="text-slate-500 p-4 text-center -mt-12">Click on a card to open project page</p>
   <div class="grid grid-cols-1 md:grid-cols-2 gap-6 sm:gap-8 px-2 sm:px-8 [&>*:last-child]:md:col-span-2 [&>*:last-child]:md:max-w-[calc(50%-1rem)] [&>*:last-child]:md:justify-self-center">
     {#each projects as project}
     <a class="flex" href={project.url} target="_blank" rel="noopener noreferrer">
       <div class="cursor-pointer bg-gradient-to-tr from-slate-900 to-slate-800 rounded-xl overflow-hidden shadow-md transition-all duration-300 hover:shadow-xl hover:-translate-y-2">
         <img src={project.image} alt={project.title} class="w-full h-48 sm:h-56 object-cover" />
         <div class="p-4 sm:p-6">
           <h3 class="text-xl sm:text-2xl font-semibold text-white mb-2 sm:mb-3">{project.title}</h3>
           <p class="text-slate-100 mb-3 sm:mb-4 text-sm sm:text-base line-clamp-5">{project.description}</p>
           <div class="flex flex-wrap gap-2 mt-auto">
             {#each project.tags as tag}
               <span class="bg-sky-100 text-sky-800 px-2 py-1 rounded-full text-xs sm:text-sm font-medium mb-1">
                 {tag}
               </span>
             {/each}
           </div>
         </div>
       </div>
      </a>
     {/each}
   </div>
 </div>