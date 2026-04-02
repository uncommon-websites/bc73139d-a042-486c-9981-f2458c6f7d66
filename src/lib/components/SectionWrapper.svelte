<script lang="ts">
  type Props = {
    className?: string;
    withBorderBottom?: boolean;
    withBorderTop?: boolean;
  };

  let { className = "", withBorderBottom = true, withBorderTop = false }: Props = $props();
</script>

<div class="relative w-full max-w-[1400px] mx-auto px-4 md:px-8 {className}">
  <!-- Corner Markers -->
  {#if withBorderTop}
    <div class="absolute top-0 left-4 md:left-8 w-px h-3 bg-gray-300 -translate-y-1.5"></div>
    <div class="absolute top-0 left-4 md:left-8 w-3 h-px bg-gray-300 -translate-x-1.5"></div>
    
    <div class="absolute top-0 right-4 md:right-8 w-px h-3 bg-gray-300 -translate-y-1.5"></div>
    <div class="absolute top-0 right-4 md:right-8 w-3 h-px bg-gray-300 translate-x-1.5"></div>
    
    <div class="absolute top-0 left-4 md:left-8 right-4 md:right-8 h-px bg-gray-200"></div>
  {/if}

  <div class="relative h-full border-l border-r border-gray-200 border-dashed md:border-solid border-opacity-50 md:border-opacity-100">
    <slot />
  </div>

  {#if withBorderBottom}
    <div class="absolute bottom-0 left-4 md:left-8 w-px h-3 bg-gray-300 translate-y-1.5"></div>
    <div class="absolute bottom-0 left-4 md:left-8 w-3 h-px bg-gray-300 -translate-x-1.5"></div>
    
    <div class="absolute bottom-0 right-4 md:right-8 w-px h-3 bg-gray-300 translate-y-1.5"></div>
    <div class="absolute bottom-0 right-4 md:right-8 w-3 h-px bg-gray-300 translate-x-1.5"></div>
    
    <div class="absolute bottom-0 left-4 md:left-8 right-4 md:right-8 h-px bg-gray-200"></div>
  {/if}
</div>
