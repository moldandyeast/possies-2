# Tinker Studio

A small procedural-animation robot with no keyframes. Every pose is solved live from constraints, 3D inverse kinematics and springs. Build a looping sequence on the timeline, or direct Tinker live in Free move.

- Live: https://demo-possie-procedural-bot.moldandyeast.com
- Everything is in one file: `public/index.html`. No build step, no dependencies.

## Credits

- The stepping and constraint ideas come from [A simple procedural animation technique](https://www.youtube.com/watch?v=qlfh_rv6khY) by argonaut.
- Set in [ABC Areal](https://abcdinamo.com/typefaces/areal) by Dinamo.
- More experiments at https://content.moldandyeast.com

## Font

ABC Areal is a licensed typeface and is not included in this repo. The page expects `public/fonts/ABCArealSuperfamilyVariable.woff2` and falls back to Arial when it is missing. If you have a licence, drop the file in that folder.

## Deploy

Hosted as a Cloudflare Worker serving `public/` as static assets. The custom domain is declared in `wrangler.toml`.

```sh
npx wrangler@4 deploy
```
