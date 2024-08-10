<script>
    import ScrollingList from "./ScrollingList.svelte";
    import Header from "./Header.svelte";

    let tech_i_know = ['React', 'Node', 'React Native', 'Python', 'SQL', 'Linux', 'Flask', 'Javascript', 'Svelte', 'MongoDB']
    let things_im_learning = ['ESP32', 'Embedded Development', '3D Modelling', 'Machine Learning', 'Music Production']
   </script>
   <div class="px-12 flex flex-col min-h-96 font-serif h-screen bg-gradient-to-br from-black to-slate-800">
     <Header />
     <div class="flex-1 flex">
       <!-- Main content area (66%) -->
       <div class="flex-[2] flex items-center justify-center">
         <div id="h" class="text-white p-4 flex flex-col justify-center gap-2">
           <div class="text-7xl py-4 bg-gradient-to-r from-blue-400 to-blue-900 inline-block text-transparent bg-clip-text">
             Hi, I'm Safal!
           </div>
           <div class="text-lg text-wrap max-w-sm text-slate-200">
             A Computer Science and Anthropology Student, I'm a programmer who blah blah blah blah blah blah
           </div>
           <div class="flex gap-2 mt-10 text-xl">
             <div class="text-green-400">
               Programmer
             </div>
             <div>
               x
             </div>
             <div class="text-red-500">
               Computer Science & Anthropology Student
             </div>
           </div>
           <div>
             Social Icons
           </div>
         </div>
       </div>
       
       <!-- side component (33%) -->
       <div class="flex-1 flex flex-col justify-center p-4 text-slate-300">
        <div class="flex flex-col gap-28">
            <div>
                <h2 class="text-2xl pb-4 text-center text-slate-300">Tech I've Worked With</h2>
                <ScrollingList items={tech_i_know} />
                <div class="flex justify-center">
                    <div class="cursor-pointer border border-slate-100 hover:bg-slate-200 hover:text-slate-800 rounded-xl inline-block px-2 -mt-2 text-slate-200">See My Projects!</div>
                </div>
              </div>
              <!--
              <div>
                <h2 class="text-2xl mb-4 text-center">Things I'm Learning</h2>
                <div class="flex">
                {#each things_im_learning as thing}
                <div class="text-center border border-r-1">{thing}</div>
                {/each}
            </div>
              </div>
              -->
        </div>

       </div>
     </div>
   </div>