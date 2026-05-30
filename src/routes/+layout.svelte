<script lang="ts">
  import favicon from "$lib/assets/favicon.png";
  import icon from "$lib/assets/favicon.png";

  let { children } = $props();
</script>

<svelte:head>
  <link rel="icon" href={favicon} />

  <meta property="og:title" content="Foxscotch" />
  <meta property="og:type" content="website" />
  <meta property="og:image" content={icon} />
  <meta property="og:url" content="https://foxscot.ch/" />
</svelte:head>

{@render children()}

<style>
  :root {
    /* --- Character Palettes --- */

    --fox-pink: #ff0055;
    --fox-pink-dark: #b3003b;
    --fox-white: #ffffff;
    --fox-black: #0d0508;

    --sebastien-primary: #ff6701;
    --sebastien-primary-light: #f9b844;
    --sebastien-secondary: #353140;
    --sebastien-secondary-hl: #1e1a2b;

    --hanna-primary: #0297fe;
    --hanna-primary-dark: #0647bb;
    --hanna-secondary: #e2e6d4;
    --hanna-secondary-light: #f1f0ef;
    --hanna-secondary-dark: #cfd4c0;

    /* --- Page Colors --- */

    --primary: var(--fox-pink);
    --primary-hl: var(--fox-pink-dark);
    --secondary: var(--fox-black);
    --secondary-hl: var(--fox-white);

    --text: var(--secondary);
    --muted-text: rgba(246, 247, 243, 0.5);
    --background: var(--secondary-hl);
    --wallpaper: var(--secondary);

    font-family: "Noto Sans", sans-serif;
  }

  :global(body) {
    font-size: 1.2em;
    text-align: left;
    color: var(--text);
    background-color: var(--wallpaper);
  }
</style>
