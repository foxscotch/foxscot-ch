# foxscot.ch

This is the repository for my personal homepage, currently at
[foxscot.ch](https://foxscot.ch/). It's meant to look a little carrd-ish, at
least for now.

I'm in the process of converting it to a SvelteKit app, so I can do more
advanced stuff with it afterwards. It's currently in state that's visually
identical to the original version, but a lot is still to be done to make it
more... Sveltey. Like breaking up the single `+page.svelte` into smaller pieces.
What you see here isn't actually on the real site yet. Still the old version.

The binary font files for the fonts used are not included in this repository,
but you can get them yourself with little effort from
[Google Fonts](https://fonts.google.com/). They should be placed in
static/webfonts/, and you'll obviously have to update fonts.css if you're not
using the same two. Same goes for [FontAwesome](https://fontawesome.com/)
Brands, which I used for the brand icons.

Otherwise, you should be good to go. You should also replace the images in
src/lib/assets if you aren't me, though. And maybe change the colors.

Last but not least, the CSS reset I used is of course
[Eric A. Meyer's](https://meyerweb.com/eric/tools/css/reset/).

## Developing

Install dependencies with `pnpm install`, then start a development server:

```sh
npm run dev
```

## Building

To generate a production build:

```sh
npm run build
```
