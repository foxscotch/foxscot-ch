<script lang="ts">
  import icon from "$lib/assets/icon.png";
  import Markdown from "$lib/components/Markdown.svelte";
  import SocialMedia from "$lib/components/SocialMedia.svelte";
  import AttributedImage from "$lib/components/AttributedImage.svelte";
  import bio from "$lib/copy/fox.md?raw";
  import { FontAwesomeIcon } from "@fortawesome/svelte-fontawesome";
  import { faGithub } from "@fortawesome/free-brands-svg-icons";
</script>

<div class="main">
  <div class="icon">
    <AttributedImage
      src={icon}
      attributionLabel="Shlimaz"
      attributionUrl="https://www.furaffinity.net/view/57092610/"
      alt="White housecat furry with pink accents, making a mischievous face"
    />
  </div>
  <h1>Foxscotch</h1>
  <p class="subtitle">she ⬪ they</p>
  <SocialMedia />
  <hr />
  <Markdown text={bio} />
  <!-- I'll uncomment this when I add a section for other people's 88x31 buttons!
    <hr />
    <p class="button"><img src="/img/button.png" /></p>
  -->
</div>
<div class="footer">
  <p>
    pixel art favicon by my friend
    <a href="https://selic.re/" target="_blank">Selicre</a>
    <br />
    <a
      href="https://github.com/foxscotch/foxscot-ch"
      target="_blank"
      aria-label="link to github repo for this site"
    >
      <FontAwesomeIcon icon={faGithub} />
    </a>
  </p>
</div>

<style>
  .subtitle {
    text-align: center;
    margin-top: 0.25em;
  }

  .main {
    box-sizing: border-box;
    width: 100%;
    height: 100%;
    padding: 4rem 1rem 2rem;
    border-style: solid;
    border-color: var(--primary);
    border-width: 1rem 0rem 0rem 0rem;
    background-color: var(--background);
  }

  .icon {
    text-align: center;
    margin-bottom: 2em;
  }

  .icon :global(img) {
    border: 5px solid transparent;
    box-shadow: 1rem -1em 0rem 0rem var(--primary);
    width: 50%;
  }

  .button {
    margin-top: 4rem;
  }

  .button img {
    display: block;
    margin: auto;
    height: 62px;
    width: 176px;
    image-rendering: pixelated;
  }

  .footer {
    font-size: 0.6em;
    font-style: italic;
    text-align: center;
    color: var(--muted-text);
  }

  .footer :global(svg) {
    font-size: 1.2rem;
    margin-top: 0.6em;
    color: var(--muted-text);
  }

  @media (min-width: 576px) {
    .main {
      border: none;
      width: 500px;
      margin: 4rem auto 0.5rem;
      padding: 4rem 2rem 2rem;
      box-shadow: 1rem -1rem 0rem 0rem var(--primary);
    }
  }
</style>
