<script lang="ts">
  import { config } from "@fortawesome/fontawesome-svg-core";
  import "@fortawesome/fontawesome-svg-core/styles.css";
  import favicon from "$lib/assets/favicon.png";
  import icon from "$lib/assets/favicon.png";

  config.autoAddCss = false;

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

    /* --- Other Page Attributes --- */

    --desktop-min-width: 576px;

    font-family: "Noto Sans", sans-serif;
  }

  :global {
    body {
      font-size: 1.2em;
      text-align: left;
      color: var(--text);
      background-color: var(--wallpaper);
    }

    h1,
    h2,
    h3 {
      font-family: "PT Serif", serif;
      text-align: center;
    }

    /* Adapted from MDN content: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/hr#example */
    hr {
      border: none;
      border-top: 0.2em solid var(--primary-hl);
      color: var(--primary-hl);
      overflow: visible;
      text-align: center;
      height: 0px;
      margin: 2em auto 2em;
    }

    hr:after {
      background: var(--background);
      font-size: 1.4em;
      content: "✦";
      padding: 0 12px;
      position: relative;
      top: -16px;
    }
    /* End MDN content */

    h1 {
      font-size: 3em;
    }

    h2 {
      font-size: 1.5em;
    }

    h3 {
      font-size: 1.2em;
    }

    p {
      margin: 1em auto 1em;
      line-height: 1.2em;
    }

    a {
      color: var(--primary-hl);
    }

    a:hover {
      opacity: 75%;
    }

    @media (min-width: 576px) {
      h1 {
        font-size: 4.5em;
      }

      h2 {
        font-size: 2em;
      }

      h3 {
        font-size: 1.5em;
      }
    }
  }
</style>
