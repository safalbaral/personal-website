<script>
    import ScrollingList from "./ScrollingList.svelte";
    import Header from "./Header.svelte";
   </script>
   <div class="rounded-lg flex flex-col min-h-96 font-serif h-screen bg-gradient-to-br from-black to-slate-800">
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
        <div class="flex flex-col gap-8">
            <div>
                <h2 class="text-2xl mb-4 text-center text-slate-300">Tech I Know</h2>
                <p>Lorem Ipsum.</p>
              </div>
              <div>
                <h2 class="text-2xl mb-4 text-center">Things I'm Learning</h2>
                <ScrollingList />
              </div>
        </div>

       </div>
     </div>
   </div>