<script lang="ts">
  import SectionWrapper from './SectionWrapper.svelte';
  import SolutionBlock from './SolutionBlock.svelte';
</script>

<SectionWrapper withBorderBottom={true} className="">
  <div class="px-4 md:px-12">
    <div class="py-16 text-center">
      <h2 class="font-serif text-4xl text-gray-900">Our solutions</h2>
    </div>

    <!-- Block 1 -->
    <SolutionBlock
      label="Knowledge Indexing"
      title="Capture your expertise instantly"
      description="Turn podcasts, newsletters, courses & conversations into a living knowledge base that represents you at your best. Unify everything into a single digital mind through deep content integrations across your existing platforms and channels."
    >
      <!-- Visual for Block 1: Files -->
      <div class="relative w-full h-full flex items-center justify-center">
        <!-- Central Hub -->
        <div class="w-16 h-16 bg-white shadow-lg rounded-lg flex items-center justify-center z-10 border border-gray-100">
           <div class="w-8 h-8 rounded-sm" style="background-color: oklch(0.541 0.281 293.009);"></div>
        </div>
        
        <!-- Connected Files -->
        <div class="absolute top-1/4 left-1/4 bg-white p-3 shadow rounded border border-gray-100 animate-pulse">
            <div class="w-8 h-10 rounded flex items-center justify-center text-[10px] font-bold" style="background-color: oklch(0.943 0.029 294.588); color: oklch(0.491 0.27 292.581);">.MP3</div>
            <div class="mt-1 text-[10px] text-center">Podcast</div>
        </div>
        <div class="absolute top-1/4 right-1/4 bg-white p-3 shadow rounded border border-gray-100">
            <div class="w-8 h-10 rounded flex items-center justify-center text-[10px] font-bold text-white" style="background-color: oklch(0.38 0.189 293.745);">.PDF</div>
            <div class="mt-1 text-[10px] text-center">Course</div>
        </div>
        <div class="absolute bottom-1/4 left-1/3 bg-white p-3 shadow rounded border border-gray-100">
            <div class="w-8 h-10 rounded flex items-center justify-center text-[10px] font-bold text-white" style="background-color: oklch(0.606 0.25 292.717);">.DOCX</div>
            <div class="mt-1 text-[10px] text-center">Newsletter</div>
        </div>
         <div class="absolute bottom-1/4 right-1/3 bg-white p-3 shadow rounded border border-gray-100">
            <div class="w-8 h-10 bg-gray-200 rounded flex items-center justify-center text-[10px] font-bold text-gray-600">.TXT</div>
            <div class="mt-1 text-[10px] text-center">Articles</div>
        </div>
        
        <!-- Connecting Lines (Simplified) -->
        <svg class="absolute inset-0 w-full h-full pointer-events-none opacity-20" viewBox="0 0 400 300">
            <path d="M100 100 L200 150 M300 100 L200 150 M150 220 L200 150 M250 220 L200 150" stroke="currentColor" stroke-width="1" stroke-dasharray="4 4" />
        </svg>
      </div>
    </SolutionBlock>

    <!-- Block 2 -->
    <SolutionBlock
      label="Clone Deployment"
      title="Scale your presence everywhere"
      description="From one-on-one coaching to global mentorship, free yourself from repetitive questions to focus exclusively on high-impact work. Deploy your digital clone across web, SMS, WhatsApp, Slack, and API integrations — scaling effortlessly as your audience grows."
      reversed={true}
    >
      <!-- Visual for Block 2: UI Card -->
      <div class="bg-white rounded-lg shadow-xl p-6 w-3/4 max-w-sm border border-gray-100">
        <div class="flex items-center space-x-3 mb-4">
            <div class="w-8 h-8 rounded-full bg-gray-300 overflow-hidden">
                <img src="/generated/image-close-up-portrait-of-a-thoughtful-profes-1775157613920-2.webp" alt="Avatar" class="w-full h-full object-cover" />
            </div>
            <div class="text-xs text-gray-500">Lenny • Strategy session</div>
        </div>
        <h4 class="font-serif text-xl mb-4">Chat with Lenny's Clone</h4>
        <div class="space-y-2 mb-6">
            <div class="h-2 bg-gray-100 rounded w-full"></div>
            <div class="h-2 bg-gray-100 rounded w-5/6"></div>
            <div class="h-2 bg-gray-100 rounded w-4/6"></div>
        </div>
        <button class="w-full text-white py-2 rounded text-sm font-medium flex items-center justify-center space-x-2" style="background-color: oklch(0.491 0.27 292.581);">
            <span>Send to Your Audience</span>
            <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14 5l7 7m0 0l-7 7m7-7H3"></path></svg>
        </button>
      </div>
    </SolutionBlock>

    <!-- Block 3 -->
    <SolutionBlock
      label="Privacy-First Architecture"
      title="Own your intelligence, always"
      description="Reinvent knowledge sharing from a liability into an asset with privacy-first security by design. Every digital mind remains the exclusive property of its creator — your data is never shared or sold, protected by strict end-to-end encryption across every interaction."
    >
       <!-- Visual for Block 3: Report -->
       <div class="bg-white rounded shadow-lg p-8 w-2/3 max-w-xs border border-gray-100 relative">
          <div class="flex justify-between items-center mb-6 border-b pb-2">
              <div class="font-bold text-xs">Delphi AI</div>
              <div class="w-4 h-4 bg-black rounded-full"></div>
          </div>
          <div class="mb-4">
              <h5 class="font-bold text-sm">Digital Mind Report</h5>
              <div class="text-[10px] text-gray-400">Created for thought leaders worldwide by Delphi</div>
          </div>
          <div class="space-y-2 text-[8px] text-gray-500 leading-relaxed">
              <p>Your clone is built from your original content and updates continuously, ensuring every answer reflects your latest thinking and expertise.</p>
              <p>All interactions are encrypted end-to-end. Your knowledge remains solely yours — never shared, never sold, always under your control.</p>
          </div>
       </div>
    </SolutionBlock>
  </div>
</SectionWrapper>
