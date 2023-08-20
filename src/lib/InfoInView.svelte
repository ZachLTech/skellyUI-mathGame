<script lang="ts">
    import { inview } from 'svelte-inview';
    import type { ObserverEventDetails, Options } from 'svelte-inview';
    import Info from './Info.svelte';

    let isInView;
    const options: Options = {
      rootMargin: '50px',
      unobserveOnEnter: true,
    };
  
    const handleChange = ({ detail }: CustomEvent<ObserverEventDetails>) =>
      (isInView = detail.inView);
  </script>

  <div use:inview="{options}" on:inview_change="{handleChange}">
    {#if isInView}
      <Info />
    {:else}
      <div class="placeholder" />
    {/if}
  </div>