<script lang="ts">
  const cards = [
    {
      title: "We Don't Hand You a Binder...",
      subtitle: "We Get in the Trenches.",
      image: "/generated/image-experienced-contractor-mentoring-younger-1765515142157-5.webp"
    },
    {
      title: "We Don't Speak Consultant...",
      subtitle: "We Speak Builder.",
      image: "/generated/image-construction-business-owner-in-hardhat-r-1765515144831-6.webp"
    },
    {
      title: "We Don't Offer False Choices...",
      subtitle: "Profitability AND Sanity.",
      image: "/generated/image-contractor-at-desk-with-construction-pla-1765515147586-7.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-2xl mb-16">
    <p class="text-xl md:text-2xl leading-relaxed text-gray-800">
      We're not theorists. We're builders who became business operators. We understand the gap between being a skilled tradesperson and running a thriving company—because we've lived it.
    </p>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    {#each cards as card}
      <div class="group">
        <div class="aspect-[4/3] overflow-hidden rounded-lg mb-4 bg-gray-100">
          <img src={card.image} alt={card.title} class="w-full h-full object-cover grayscale group-hover:grayscale-0 transition-all duration-500" />
        </div>
        <h3 class="text-sm text-gray-500 mb-1">{card.title}</h3>
        <p class="text-sm font-bold">{card.subtitle}</p>
        
        <div class="flex justify-between mt-4 text-xs text-gray-400">
           <span>→</span>
           <span>Built for builders</span>
        </div>
      </div>
    {/each}
  </div>
</section>
