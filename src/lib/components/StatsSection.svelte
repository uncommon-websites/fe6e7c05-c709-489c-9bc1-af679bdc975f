<script lang="ts">
  const stats = [
    {
      label: "$300k–$10M",
      desc: "Our sweet spot. Post-startup contractors who've proven their craft but hit a growth ceiling. You're honest, hardworking, and humble enough to ask for help. You want to become better leaders, not just better managers.",
      img: ""
    },
    {
      label: "Triage-First Model",
      desc: "We don't follow the playbook. We identify your 'bleeding neck'—the most critical issue—and solve it first. This creates immediate impact and momentum. No theory, no binders, just results.",
      img: ""
    },
    {
      label: "Operator-Led Systems",
      desc: "We're not consultants who disappear after handing you advice. We're operators who implement JobTread, CompanyCam, and ClickUp, then stay with you through the transformation. We get in the trenches.",
      img: ""
    },
    {
      label: "Inside-Out Approach",
      desc: "You can't fix a business if the leader is broken. We address imposter syndrome, burnout, and identity crisis alongside business metrics. This is human-centered consulting for the trades.",
      img: ""
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white border-t border-gray-100">
  <div class="mb-16">
    <p class="text-gray-500 max-w-xl">
      We work with contractors who excel at their craft but need help with the business side. Here's what makes us different.
    </p>
  </div>

  <div class="space-y-16">
    {#each stats as stat}
      <div class="flex flex-col md:flex-row md:items-start justify-between gap-8 border-b border-gray-100 pb-16 last:border-0">
        <h3 class="text-2xl md:text-4xl font-medium w-full md:w-1/3">{stat.label}</h3>
        <div class="w-full md:w-1/3">
           <p class="text-xs leading-relaxed text-gray-500">{stat.desc}</p>
        </div>
        <div class="w-full md:w-1/6 flex justify-end">
           {#if stat.img}
             <img src={stat.img} alt={stat.label} class="w-20 h-20 object-cover rounded bg-gray-100" />
           {:else}
             <div class="w-20 h-20 rounded bg-gray-100 flex items-center justify-center">
               <div class="w-8 h-8 border-2 border-gray-300 rounded"></div>
             </div>
           {/if}
        </div>
      </div>
    {/each}
  </div>
</section>
