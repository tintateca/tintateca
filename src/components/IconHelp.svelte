<script>
  import { onMount } from 'svelte';
  let iconVisible = true;

  onMount(() => {
      const timer = setInterval(() => {
        iconVisible = !iconVisible;
      }, 1000); 
      return () => clearInterval(timer);
  });
</script>

<div class="icon-container">
  <a href="https://wa.me/+34666698128?text=Hello%20there!" aria-label="Contact Us" class={iconVisible ? 'block' : 'hidden'} target="_blank">
    <svg width="40"  height="40"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-brand-whatsapp">
      <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
      <path d="M3 21l1.65 -3.8a9 9 0 1 1 3.4 2.9l-5.05 .9" />
      <path d="M9 10a.5 .5 0 0 0 1 0v-1a.5 .5 0 0 0 -1 0v1a5 5 0 0 0 5 5h1a.5 .5 0 0 0 0 -1h-1a.5 .5 0 0 0 0 1" />
    </svg>
  </a>
</div>
