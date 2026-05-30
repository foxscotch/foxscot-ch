<script lang="ts">
  import icon from "$lib/assets/icon.png";
</script>

<div class="main">
  <div class="icon">
    <img
      src={icon}
      alt="White cat furry with pink accents, making a >:3 face"
    />
  </div>
  <h1>Foxscotch</h1>
  <p class="subtitle">she ⬪ they</p>
  <div class="social-media">
    <a
      href="https://t.me/foxscotch"
      target="_blank"
      aria-label="link to telegram profile"
    >
      <i class="fa-brands fa-fw fa-telegram"></i>
    </a>
    <a
      href="https://foxscotch.tumblr.com/"
      target="_blank"
      aria-label="link to tumblr profile"
    >
      <i class="fa-brands fa-fw fa-tumblr"></i>
    </a>
    <a
      href="https://bsky.app/profile/foxscot.ch"
      target="_blank"
      aria-label="link to bluesky profile"
    >
      <i class="fa-brands fa-fw fa-bluesky"></i>
    </a>
    <a
      href="https://twitter.com/foxscotch"
      target="_blank"
      aria-label="link to twitter profile"
    >
      <i class="fa-brands fa-fw fa-twitter"></i>
    </a>
    <a
      href="https://steamcommunity.com/id/foxscotch"
      target="_blank"
      aria-label="link to steam profile"
    >
      <i class="fa-brands fa-fw fa-steam"></i>
    </a>
  </div>
  <div class="social-media discord">
    <i class="fa-brands fa-fw fa-discord"></i> @foxscotch
  </div>
  <hr />
  <p>
    Hi, I'm Foxscotch! Feel free to call me Fox or Scotch if you'd like. I'm a <a
      href="https://www.furaffinity.net/view/56828476/">cat</a
    >.
  </p>
  <p>
    I love animals, especially, obviously, cats. Also a big insect fan, with a
    particular fascination for ants and wasps. But really, there's no animal I
    don't like! And I mean that.
  </p>
  <p>
    My hobbies include programming, a bit of 3D modeling, and sometimes playing
    video games. Programming is also what I do for work! Specifically web
    development.
  </p>
  <p>
    Feel free to hit me up on any of the social media platforms linked up top.
    Telegram is best, but they'll all get you a response eventually.
  </p>
  <hr />
  <p>
    The art for the icon above was drawn by
    <a href="https://www.furaffinity.net/view/57092610/">Shlimaz</a>, and the
    pixel art in the favicon is from my friend
    <a href="https://selic.re/">Selicre</a>.
  </p>
  <!-- I'll uncomment this when I add a section for other people's 88x31 buttons!
        <hr />
        <p class="button"><img src="/img/button.png" /></p>
      -->
</div>
<div class="footer">
  <div class="footer-item center">
    <p>
      &copy; Foxscotch
      <br />
      <a
        href="https://github.com/foxscotch/foxscot-ch"
        target="_blank"
        aria-label="link to github repo for this site"
      >
        <i class="fa-brands fa-github"></i>
      </a>
    </p>
  </div>
</div>

<style>
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
  }

  .icon > img {
    margin-bottom: 2em;
    border: 5px solid transparent;
    box-shadow: 1rem -1em 0rem 0rem var(--primary);
    width: 50%;
  }

  .social-media {
    text-align: center;
  }

  .social-media a {
    color: var(--text);
    text-decoration: none;
    margin-right: 1em;
  }

  .social-media a:last-child {
    margin-right: 0;
  }

  .social-media.discord {
    font-size: 0.8em;
    margin-top: 0.6em;
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

  .footer,
  .footer i {
    text-align: center;
    line-height: 2rem;
    color: var(--muted-text);
  }

  .pt-serif {
    font-family: "PT Serif", serif;
  }

  .noto-sans {
    font-family: "Noto Sans", sans-serif;
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

    .main {
      border: none;
      width: 500px;
      margin: 4rem auto 1rem;
      padding: 4rem 2rem 2rem;
      box-shadow: 1rem -1rem 0rem 0rem var(--primary);
    }
  }
</style>
