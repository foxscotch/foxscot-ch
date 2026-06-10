<script lang="ts">
  import { FontAwesomeIcon } from "@fortawesome/svelte-fontawesome";
  import {
    faBluesky,
    faDiscord,
    faSteam,
    faTelegram,
    faTumblr,
    faTwitter,
  } from "@fortawesome/free-brands-svg-icons";
</script>

<div class="social-media">
  <a
    href="https://t.me/foxscotch"
    target="_blank"
    aria-label="link to telegram profile"
  >
    <FontAwesomeIcon icon={faTelegram} />
  </a>
  <a
    href="https://foxscotch.tumblr.com/"
    target="_blank"
    aria-label="link to tumblr profile"
  >
    <FontAwesomeIcon icon={faTumblr} />
  </a>
  <a
    href="https://bsky.app/profile/foxscot.ch"
    target="_blank"
    aria-label="link to bluesky profile"
  >
    <FontAwesomeIcon icon={faBluesky} />
  </a>
  <a
    href="https://twitter.com/foxscotch"
    target="_blank"
    aria-label="link to twitter profile"
  >
    <FontAwesomeIcon icon={faTwitter} />
  </a>
  <a
    href="https://steamcommunity.com/id/foxscotch"
    target="_blank"
    aria-label="link to steam profile"
  >
    <FontAwesomeIcon icon={faSteam} />
  </a>
</div>
<p class="social-media-discord">
  <FontAwesomeIcon icon={faDiscord} /> @foxscotch
</p>

<style>
  .social-media {
    display: flex;
    justify-content: center;
    flex-direction: row;
    gap: 1.25em;
  }

  .social-media a {
    color: var(--text);
    text-decoration: none;
  }

  .social-media-discord {
    text-align: center;
    font-size: 0.8em;
  }
</style>
