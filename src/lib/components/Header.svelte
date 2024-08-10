<div class="sticky top-0 w-full flex items-center justify-between p-4 md:p-8 font-serif text-lg text-slate-200">
  <div id="logo">
    <img src="/src/assets/Logo.png" class="w-16 h-16 md:w-20 md:h-20" alt="Logo" />
  </div>
  <div id="nav-items" class="flex gap-4 md:gap-6">
    <a class="hover-underline-animation cursor-pointer" href="#projects">
      Projects
    </a>
    <a class="hover-underline-animation cursor-pointer" href="#experience">
      Experience
    </a>
  </div>
</div>

<style>
  .hover-underline-animation {
    display: inline-block;
    position: relative;
    padding-bottom: 2px; /* Add padding to create space for the underline */
  }

  .hover-underline-animation::after {
    content: '';
    position: absolute;
    width: 100%;
    transform: scaleX(0);
    height: 2px;
    bottom: 0;
    left: 0;
    background-color: white;
    transform-origin: bottom right;
    transition: transform 0.25s ease-out;
  }

  .hover-underline-animation:hover::after {
    transform: scaleX(1);
    transform-origin: bottom left;
  }
</style>