<script lang="ts">
  type Props = {
    label: string;
    title: string;
    description: string;
    linkText?: string;
    linkHref?: string;
    reversed?: boolean;
  };

  let { label, title, description, linkText = "Discover more", linkHref = "#", reversed = false }: Props = $props();
</script>

<div class="flex flex-col md:flex-row items-center gap-12 md:gap-20 py-16 md:py-24 border-b border-gray-200 border-dashed last:border-0">
  <!-- Text Content -->
  <div class="flex-1 {reversed ? 'md:order-2' : 'md:order-1'}">
    <div class="text-xs font-mono uppercase tracking-widest text-gray-500 mb-4">
      {label}
    </div>
    <h3 class="font-serif text-4xl text-gray-900 mb-6">
      {title}
    </h3>
    <p class="text-gray-500 leading-relaxed mb-8 max-w-md">
      {description}
    </p>
    <a href={linkHref} class="font-medium hover:underline text-sm" style="color: oklch(0.541 0.281 293.009);">
      {linkText}
    </a>
  </div>

  <!-- Visual Content -->
  <div class="flex-1 w-full {reversed ? 'md:order-1' : 'md:order-2'}">
    <div class="bg-gray-50 rounded-lg p-8 md:p-12 aspect-[4/3] flex items-center justify-center relative overflow-hidden">
      <slot />
    </div>
  </div>
</div>
