<script>
    import ScrollingList from "./ScrollingList.svelte";
    import Header from "./Header.svelte";
    let tech_i_know = ['React', 'Node', 'React Native', 'Python', 'SQLite', 'Linux', 'Flask', 'Javascript', 'Svelte', 'MongoDB', 'TailwindCSS']
    let things_im_learning = ['ESP32', 'Embedded Development', '3D Modelling', 'Machine Learning', 'Music Production']
   </script>
   
   <div class="px-4 sm:px-12 flex flex-col min-h-screen font-serif bg-gradient-to-br from-black to-slate-800">
     <Header />
     <div class="flex-1 flex flex-col md:flex-row justify-center">
       <!-- Main content area -->
       <div class="md:flex-[2] flex items-center justify-center">
         <div class="text-white p-4 flex flex-col justify-center gap-2">
           <h1 class="text-5xl sm:text-6xl md:text-7xl py-4 bg-gradient-to-r from-blue-400 to-blue-900 inline-block text-transparent bg-clip-text">
             Hi, I'm Safal!
           </h1>
           <p class="text-base sm:text-lg text-wrap max-w-sm text-slate-200">
            Jack of all trades, hoping to be a master at some. I enjoy exploring new subjects and hobbies, from the command line to human culture.
           </p>
           <p class="text-base text-wrap max-w-sm text-slate-200">
            Some things I'm learning: <span class="text-slate-300 text-sm">Embedded Development, Machine Learning, Woodworking, Video Production</span>
           </p>
           <div class="flex gap-2 py-2 sm:py-5 md:py-10 text-base sm:text-lg md:text-xl">
             <span class="text-green-400">Programmer</span>
             <span>x</span>
             <span class="text-red-500">Computer Science & Anthropology Student</span>
           </div>
           <div class="flex gap-4">
            <a href="https://github.com/safalbaral/" target="_blank" rel="noopener noreferrer">
                <ion-icon name="logo-github" style="font-size: 24px;"></ion-icon>
            </a>
            <a href="#" target="_blank" rel="noopener noreferrer">
                <ion-icon name="logo-linkedin" style="font-size: 24px;"></ion-icon>
            </a>
            <a href="#" target="_blank" rel="noopener noreferrer">
                <ion-icon name="mail" style="font-size: 24px;"></ion-icon>
            </a>
           </div>
         </div>
       </div>
       <!-- Side component -->
       <div class="md:flex-1 flex flex-col justify-center p-4 text-slate-300 mt-8 md:mt-0">
         <div class="flex flex-col gap-8 md:gap-28">
           <div>
             <h2 class="text-xl sm:text-2xl pb-4 text-center text-slate-300">Tech I've Worked With</h2>
             <ScrollingList items={tech_i_know} />
             <div class="flex justify-center mt-4">
               <a href="#projects" class="cursor-pointer border border-slate-100 hover:bg-slate-200 hover:text-slate-800 rounded-xl px-4 py-2 text-slate-200">See My Projects!</a>
             </div>
           </div>
           <!--
           <div>
             <h2 class="text-xl sm:text-2xl mb-4 text-center">Things I'm Learning</h2>
             <div class="flex flex-wrap justify-center gap-2">
               {#each things_im_learning as thing}
                 <div class="text-center border border-slate-300 px-2 py-1 rounded">{thing}</div>
               {/each}
             </div>
           </div>
           -->
         </div>
       </div>
     </div>
   </div>