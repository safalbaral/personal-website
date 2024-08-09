<script>
    let technologies = [
      'JavaScript', 'TypeScript', 'React', 'Vue', 'Angular',
      'Node.js', 'Express', 'MongoDB', 'PostgreSQL', 'GraphQL',
      'Docker', 'Kubernetes', 'AWS', 'Firebase', 'Redux',
      'Webpack', 'Babel', 'Jest', 'Cypress', 'Git'
    ];
  
    // Duplicate the list to create a seamless loop
    technologies = [...technologies, ...technologies];
  </script>
  <div class="overflow-hidden h-full relative">
    <div class="animate-scroll absolute left-0 flex">
      {#each technologies as tech}
        <div class="py-4 px-4 whitespace-nowrap text-xl font-bold text-gray-500">{tech}</div>
      {/each}
    </div>
  </div>
  
  <style>
    @keyframes scroll {
      0% {
        transform: translateX(0);
      }
      100% {
        transform: translateX(-30%);
      }
    }
  
    .animate-scroll {
      animation: scroll 60s linear infinite;
    }
  </style>