<script>
    let projects = [
      { 
        title: 'App', 
        description: 'A brief description of project 1. Lorem Ipsum.',
        tags: ['React Native', 'Tag'],
        image: '/images/project1.jpg'
      },
      { 
        title: 'HERD Project', 
        description: 'A brief description of project 2. Lorem Ipsum.',
        tags: ['Tag', 'Tag'],
        image: '/images/project2.jpg'
      },
      { 
        title: 'SUTD DTI', 
        description: 'A brief description of project 3. Lorem Ipsum.',
        tags: ['Tag', 'Tag'],
        image: '/images/project3.jpg'
      },
      { 
        title: 'Billing', 
        description: 'A brief description of the project. Lorem Ipsum',
        tags: ['Python', 'Flask'],
        image: '/images/project4.jpg'
      },
      { 
        title: 'Project 5', 
        description: 'A brief description of the project. Lorem Ipsum.',
        tags: ['IoT', 'Arduino'],
        image: '/images/project5.jpg'
      },
      { 
        title: 'Project 6', 
        description: 'A brief description of the project. Lorem Ipsum.',
        tags: ['Tag', 'Tag'],
        image: '/images/project6.jpg'
      },
    ];
   </script>
   
   <div id="projects" class="font-sans bg-gradient-to-tr from-black to-slate-800 p-8">
     <h2 class="py-2 text-5xl font-bold text-white mb-12 text-center bg-gradient-to-r from-blue-50 to-blue-700 text-transparent bg-clip-text">Projects</h2>
     <div class="grid grid-cols-1 md:grid-cols-2 gap-8 px-36">
       {#each projects as project}
         <div class="cursor-pointer bg-gradient-to-tr from-slate-900 to-slate-800 rounded-xl overflow-hidden shadow-md transition-all duration-300 hover:shadow-xl hover:-translate-y-2">
           <img src={project.image} alt={project.title} class="w-full h-48 object-cover" />
           <div class="p-6">
             <h3 class="text-2xl font-semibold text-white mb-3">{project.title}</h3>
             <p class="text-slate-100 mb-4 line-clamp-3">{project.description}</p>
             <div class="flex flex-wrap gap-2 mt-auto">
               {#each project.tags as tag}
                 <span class="bg-sky-100 text-sky-800 px-3 py-1 rounded-full text-sm font-medium">
                   {tag}
                 </span>
               {/each}
             </div>
           </div>
         </div>
       {/each}
     </div>
   </div>