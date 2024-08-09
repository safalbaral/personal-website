<div class="sticky mt-0 w-full flex justify-between p-8 font-serif text-lg text-slate-200">
    <div id="logo">
        Logo Here
    </div>
    <div id="nav-items" class="flex gap-6">
        <a class="hover-underline-animation cursor-pointer" href="#projects">
            Projects
        </a>
        <div class="hover-underline-animation cursor-pointer">
            Experience
        </div>
    </div>
</div>

<style>
.hover-underline-animation {
  display: inline-block;
  position: relative;
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