<script lang="ts">
  import { toCamelCase } from '$lib/shared/app';
  
  export let label: string;
</script>

<div class="grid grid-cols-none md:grid-cols-4 gap-2 md:gap-3 lg:gap-5 mt-5 items-center form-control">
  <label for={toCamelCase(label)} class="md:text-xl md:col-span-4 xl:col-span-1">{label}</label>
  <slot />
</div>

