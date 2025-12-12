<script lang="ts">
  // Trade associations and industry partners
  const associations = [
    "AGC",
    "NAHB",
    "ABC",
    "NECA",
    "PHCC"
  ];
</script>

<section class="relative min-h-screen flex flex-col justify-end pb-20 px-6 md:px-12 bg-gradient-to-b from-black via-gray-800 to-white text-[#1a1a1a]">
  <!-- Gradient overlay/background handling -->
  <div class="absolute inset-0 z-[-1] bg-[linear-gradient(180deg,#000_0%,#1a1a1a_30%,#4a4a4a_60%,#fff_100%)]"></div>

  <div class="max-w-4xl mb-32 pt-40">
    <h1 class="text-3xl md:text-5xl font-medium leading-[1.15] tracking-tight">
      Transform chaos into profit through operational triage and inside-out leadership. <span class="text-gray-500">We speak your language. We've been in the trenches. We help contractors earning $300k–$10M scale without breaking.</span>
    </h1>
  </div>

  <div class="border-t border-gray-300 pt-8 flex flex-wrap gap-8 md:gap-16 items-center opacity-60">
    <p class="text-xs uppercase tracking-wider text-gray-600 font-medium">Trusted by contractors nationwide</p>
    {#each associations as association}
      <div class="h-8 flex items-center justify-center font-bold text-lg text-gray-700">{association}</div>
    {/each}
  </div>
</section>
