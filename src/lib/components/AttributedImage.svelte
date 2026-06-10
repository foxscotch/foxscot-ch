<script lang="ts">
  import type { HTMLImgAttributes } from "svelte/elements";

  type Props = HTMLImgAttributes & {
    attributionLabel: string;
    attributionUrl?: string;
  };

  let { attributionLabel, attributionUrl, ...rest }: Props = $props();
</script>

<figure>
  <img {...rest} />
  <figcaption>
    art by
    {#if attributionUrl}
      <a href={attributionUrl} rel="external" target="_blank">
        {attributionLabel}
      </a>
    {:else}
      {attributionLabel}
    {/if}
  </figcaption>
</figure>

<style>
  figcaption {
    margin-top: 0;
    font-style: italic;
    font-size: 0.6em;
  }
</style>
