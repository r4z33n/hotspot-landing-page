## Run the project

```bash
npm i
npm run  dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

Make sure you have the [eslint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) and [prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) extensions installed on vscode.

## Things you need to replace

In no particular order, here are the things you should look into changing to make the site your own:

- Change the images on the site (including the social image embedded when sharing the url, saved as `opengraph-image.png`)

- Change all the copywriting and text on the homepage

- Change the terms of service & privacy policy to yours

- Add whatever you want to your header by modifying the `items` array in `header.tsx`

- Replace the theme in `src/app/global.css` with your own shadcn theme, which you can [generate here](https://ui.shadcn.com/themes) by choosing your colors and clicking `copy code`. Note I created a new color called `minor` which isn't native to shadcn, so you may need to add a replacement for that on some typographys

- Replace the SEO metadata and titles in `layout.tsx`

- Replace all the links with whatever you want
- There's also a husky integration I added, feel free to set that up by running `npx husky install`

## Next steps to build a SaaS from this repo

If you're building a full SaaS off of this repo, here's what you should look into doing next, depending on what you need:

- If you need any environment variables, create a `.env.local` and use them in standard NextJS style

- Create the login / signup logic. I'd personally recommend using [Supabase <> NextJS's integration](https://supabase.com/docs/guides/auth/quickstarts/nextjs), since it's super simple and quick to setup

- Logic to show different header items for someone logged in vs someone not (if your app needs it)

- Additional components if you're modifying the homepage

- If you're SaaS has already launched, you can add more elements to the landing page like customer testimonials, demos, etc. A full list of things I'd recommend is [here](https://map.sistilli.dev/public/startups/concepts/SaaS+Landing+Page+Design+Standards)

- Code the rest of your SaaS!
- Create more designs on figma (see section below)

## Design on Figma

I have the accompanying [Figma file here](https://www.figma.com/community/file/1366853311251031961) so you can fork it and build out your SaaS from it while keeping the styles consistent.

If you're a developer that's new to Figma, [here's my crashcourse on Figma for developers](https://www.youtube.com/watch?v=Vw_XmufXCCI).

If you ended up changing the shadcn theme, you can modify the color variables on Figma to match your code. Same for typography variants.

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.

Basically:

1. Clone the repo, and push your changes up

2. Log into your Vercel account

3. Create a new project, link your repo, and it will auto deploy

Depending on what you modify, you may have build issues what prevent your site from deploying, but generally it should work out of the box. Any issues that do come up are usually super obvious and easy to solve by looking at the build failure logs.

I'd also recommend buying a domain on a platform like Cloudflare, and configuring it to point to Vercel. [Docs about that here.](https://vercel.com/docs/integrations/external-platforms/cloudflare)

## Join our community & say thanks

You can join our [Tech Founder's Discord](https://discord.gg/JNc6uPUqUU), and check out my other [socials](https://linktr.ee/anthonysistilli).

Also, if you're a tech founder like myself, feel free to subscribe on [Youtube](https://www.youtube.com/@anthonysistilli), and check out my [mind map](https://map.sistilli.dev/public/coding/SaaS+Boilerplate) where I write about startups, coding, and other things.

## Contribute

If you have any suggestions or changes, feel free to create a PR!
