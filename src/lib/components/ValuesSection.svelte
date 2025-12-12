<script lang="ts">
  const technologies = [
    {
      title: "JobTread",
      desc: "Project management and workflow automation that actually works for contractors. We implement it, train your team, and ensure adoption.",
      img: "/generated/image-smartphone-showing-construction-project--1765515228510-0.webp"
    },
    {
      title: "CompanyCam",
      desc: "Visual documentation and communication that keeps everyone on the same page. No more lost photos or miscommunication.",
      img: "/generated/image-contractor-taking-photo-documentation-of-1765515231149-1.webp"
    },
    {
      title: "ClickUp",
      desc: "Task management and team coordination that reduces chaos. Know what's happening without constant check-ins.",
      img: "/generated/image-construction-team-reviewing-task-list-on-1765515233835-2.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-xl mb-16">
    <h3 class="text-lg font-bold mb-2">Technology that creates freedom, not frustration.</h3>
    <p class="text-gray-500 text-sm leading-relaxed">
      We don't just recommend tools—we install them, integrate them, and train your team. These systems reduce site visits, automate workflows, and give you back your life. Plus fractional CFO services to transform messy books into actionable intelligence.
    </p>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    {#each technologies as tech}
      <div>
        <div class="aspect-[3/4] rounded-lg overflow-hidden mb-4 bg-gray-100">
          <img src={tech.img} alt={tech.title} class="w-full h-full object-cover" />
        </div>
        <h4 class="text-xs font-bold mb-1">{tech.title}</h4>
        <p class="text-[10px] text-gray-500 leading-relaxed">{tech.desc}</p>
      </div>
    {/each}
  </div>
</section>
