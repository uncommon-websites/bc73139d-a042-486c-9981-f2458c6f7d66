<script lang="ts">
  import SectionWrapper from './SectionWrapper.svelte';
</script>

<SectionWrapper withBorderBottom={true} className="py-24">
  <div class="px-4 md:px-12 flex flex-col md:flex-row items-center justify-between gap-12">
    <!-- Text -->
    <div class="w-full md:w-1/2">
      <h2 class="font-serif text-3xl md:text-4xl text-gray-900 mb-6">
        Privacy-first architecture as standard
      </h2>
      <p class="text-gray-500 mb-2">Your data. Your digital mind. Your control.</p>
      <p class="text-gray-500 mb-2">Never shared, sold, or used to train other models.</p>
      <p class="text-gray-500 mb-8">Enterprise-grade encryption protecting every clone, around the clock.</p>
      
      <a href="#" class="font-medium hover:underline text-sm" style="color: oklch(0.541 0.281 293.009);">
        Learn more
      </a>
    </div>

    <!-- Badges -->
    <div class="w-full md:w-1/2 flex justify-center md:justify-end gap-6">
      <!-- Badge 1 -->
      <div class="w-24 h-24 rounded-full bg-gray-100 flex flex-col items-center justify-center text-center p-2">
        <div class="text-[10px] font-bold text-gray-900 mb-1">AICPA</div>
        <div class="text-[10px] text-gray-500">SOC 2</div>
      </div>

      <!-- Badge 2 -->
      <div class="w-24 h-24 rounded-full bg-gray-100 flex flex-col items-center justify-center text-center p-2 relative border border-dashed border-gray-300">
        <div class="absolute inset-0 rounded-full border border-dashed border-gray-400 animate-spin-slow"></div>
        <div class="text-[10px] font-bold text-gray-900">GDPR</div>
        <!-- Stars visual approximation -->
        <div class="absolute inset-0 flex items-center justify-center pointer-events-none">
             <div class="w-16 h-16 border border-dotted border-gray-400 rounded-full"></div>
        </div>
      </div>

      <!-- Badge 3 -->
      <div class="w-24 h-24 rounded-full bg-gray-100 flex flex-col items-center justify-center text-center p-2">
        <div class="mb-1">
             <svg class="w-4 h-4 text-gray-900 mx-auto" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
        </div>
        <div class="text-[10px] font-bold text-gray-900">Cyber</div>
        <div class="text-[10px] text-gray-500">Essentials</div>
      </div>
    </div>
  </div>
</SectionWrapper>
