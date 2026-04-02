<script lang="ts">
  import SectionWrapper from './SectionWrapper.svelte';
</script>

<SectionWrapper withBorderBottom={true} className="py-24">
  <div class="px-4 md:px-12 max-w-4xl mx-auto text-center mb-16">
    <div class="text-xs font-mono uppercase tracking-widest text-gray-500 mb-4">
      Integrations
    </div>
    <h2 class="font-serif text-4xl text-gray-900 mb-6">
      Bring your knowledge wherever your audience is
    </h2>
    <p class="text-gray-500 leading-relaxed max-w-2xl mx-auto">
      Seamless integrations across web embeds, SMS, WhatsApp, Slack, and custom APIs ensure your digital clone is always present, always on, and always yours.
    </p>
  </div>

  <div class="px-4 md:px-12 relative">
    <!-- Connecting Line -->
    <div class="absolute top-1/2 left-0 w-full h-px bg-gray-200 -translate-y-1/2 hidden md:block"></div>

    <!-- Logos Row -->
    <div class="flex flex-wrap md:flex-nowrap items-center justify-center md:justify-between gap-8 relative z-10">
      
      <!-- Logo 1 -->
      <div class="w-16 h-16 bg-white rounded-full shadow-sm border border-gray-100 flex items-center justify-center p-3">
        <div class="text-[10px] font-bold text-gray-400">Slack</div>
      </div>

       <!-- Logo 2 -->
      <div class="w-16 h-16 bg-white rounded-full shadow-sm border border-gray-100 flex items-center justify-center p-3">
        <div class="text-[10px] font-bold text-blue-500">WhatsApp</div>
      </div>

       <!-- Center Logo (Delphi) -->
      <div class="w-24 h-24 rounded-full shadow-lg border-4 border-white flex items-center justify-center p-2 relative" style="background-color: oklch(0.38 0.189 293.745);">
        <div class="text-white font-serif font-bold text-xs tracking-widest">DELPHI</div>
        <!-- Orbit ring visual -->
        <div class="absolute inset-0 rounded-full scale-110 opacity-50" style="border: 1px solid oklch(0.491 0.27 292.581);"></div>
      </div>

       <!-- Logo 3 -->
      <div class="w-16 h-16 bg-white rounded-full shadow-sm border border-gray-100 flex items-center justify-center p-3">
        <div class="text-[10px] font-bold text-green-600">SMS</div>
      </div>

       <!-- Logo 4 -->
      <div class="w-16 h-16 bg-white rounded-full shadow-sm border border-gray-100 flex items-center justify-center p-3">
        <div class="text-[10px] font-bold text-blue-400">API</div>
      </div>

    </div>
  </div>
</SectionWrapper>
