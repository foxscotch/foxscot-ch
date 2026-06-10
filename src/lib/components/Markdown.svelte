<script lang="ts">
  import { marked } from "marked";

  let { text }: { text: string } = $props();
</script>

<!-- eslint-disable-next-line svelte/no-at-html-tags -->
{@html marked.parse(text)}
