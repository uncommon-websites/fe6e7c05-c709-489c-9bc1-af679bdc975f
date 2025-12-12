<script lang="ts">
  const services = [
    {
      title: "Operational Triage",
      desc: "We identify your 'bleeding neck'—the most critical issue—and solve it first. No theory, just immediate impact.",
      bg: "bg-black",
      img: "",
      dark: true
    },
    {
      title: "Systems Implementation",
      desc: "JobTread, CompanyCam, ClickUp—we don't just recommend tools, we install them and make them work for your team.",
      bg: "bg-gray-100",
      img: "/generated/image-contractor-reviewing-blueprints-at-a-con-1765515128817-0.webp",
      dark: false
    },
    {
      title: "Leadership Development",
      desc: "You can't fix a business if the leader is broken. We address imposter syndrome, burnout, and identity alongside metrics.",
      bg: "bg-gray-900",
      img: "/generated/image-construction-business-owner-in-their-off-1765515131903-1.webp",
      dark: true
    },
    {
      title: "Fractional CFO Services",
      desc: "Transform messy books into actionable intelligence. Understand your true margins, not just top-line revenue.",
      bg: "bg-white border border-gray-200",
      img: "",
      dark: false
    },
    {
      title: "General Contractors",
      desc: "From reactive firefighting to confident, visionary leadership. Build a business that thrives without your constant presence.",
      bg: "bg-gray-100",
      img: "/generated/image-contractor-using-tablet-on-job-site-to-d-1765515134510-2.webp",
      dark: false,
      full: true
    },
    {
      title: "Subcontractors",
      desc: "Excel at your craft while we handle the business fundamentals—contracts, insurance, cash flow, and team coordination.",
      bg: "bg-gray-50",
      img: "/generated/image-two-contractors-collaborating-and-review-1765515137009-3.webp",
      dark: false
    },
    {
      title: "Remodeling Companies",
      desc: "Scale your remodeling business with systems that reduce site visits and automate workflows without sacrificing quality.",
      bg: "bg-gray-100",
      img: "/generated/image-contractor-working-on-residential-remode-1765515139618-4.webp",
      dark: false
    }
  ];
</script>

<section class="px-6 md:px-12 py-24 bg-white">
  <div class="max-w-3xl mb-16">
    <h2 class="text-2xl md:text-3xl font-medium leading-tight">
      <span class="font-bold">We're operators, not consultants.</span> We get in the trenches to triage the mess, implement systems that create freedom, and develop leaders who can scale without breaking.
    </h2>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-2 gap-x-6 gap-y-12">
    {#each services as service}
      <div class="group cursor-pointer {service.full ? 'md:col-span-2' : ''}">
        <div class={`aspect-[4/3] w-full rounded-lg overflow-hidden relative ${service.bg} mb-4 ${service.full ? 'md:aspect-[2.5/1]' : ''}`}>
          {#if service.img}
             <img src={service.img} alt={service.title} class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105" />
          {:else}
             <!-- Icon/graphic placeholder -->
             <div class="w-full h-full flex items-center justify-center">
                <div class={`w-16 h-16 border-2 ${service.dark ? 'border-white' : 'border-black'} rounded`}></div>
             </div>
          {/if}
        </div>
        <h3 class="text-sm font-bold mb-1">{service.title}</h3>
        <p class="text-sm text-gray-600">{service.desc}</p>
      </div>
    {/each}
  </div>
</section>
