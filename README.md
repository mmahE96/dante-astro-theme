# Detailed Explanation of How the Astro Blog Works

Introduction
Astro allows usage of components in React, Vue, and Astro itself.
TypeScript is included by default.
Supports Server-Side Rendering (SSR).
Adapters available for Vercel and Node.js for deployment.

Key Features
Zero JavaScript output.
Utilizes island architectures.
Renders HTML on the server.
Allows placeholders around dynamic regions.
Combining SSR and CSR
Combines the best of SSR and CSR.
Ideal for Single Page Applications (SPA).

Component Usage
Components include .astro tags.
Compatible with React components.

Use Cases
Suitable for static websites and super-fast pre-rendered sites.
Ideal for SSR websites and web APIs.
CMS Sanity recommended for Astro apps.

Development Setup
Requires Node Package Manager (NPM).
Astro.config file contains adapters.
Run npx add astro tailwind to add Tailwind to the project.

File-Based Routing
Pages in the PAGES folder act as separate pages with built-in routing.
Tailwind templates available for styling.
Optimize images from the src folder.

Image Handling
Import images from the src folder for optimization.
Use public folder images directly as the source.
Separate Astro element IMAGE for public folder images.

Components Script
Utilize CODE FENCE as a tag for component scripts.
---
code fence
---

Write JavaScript for server-side functionality.
Frontend client-side JavaScript added using <script> tags.





# Dante - Astro & Tailwind CSS Theme by justgoodui.com

Dante is a single-author blog and portfolio theme for Astro.js. Featuring a minimal, slick, responsive and content-focused design. For more Astro.js themes please check [justgoodui.com](https://justgoodui.com/).

![Dante Astro.js Theme](public/dante-preview.jpg)

## Theme Features:

- ✅ Dark and light color mode
- ✅ Hero section with bio
- ✅ Portfolio collection
- ✅ Pagination support
- ✅ Post tags support
- ✅ Subscription form
- ✅ View transitions
- ✅ Tailwind CSS
- ✅ Mobile-first responsive layout
- ✅ SEO-friendly with canonical URLs and OpenGraph data
- ✅ Sitemap support
- ✅ RSS Feed support
- ✅ Markdown & MDX support

## Template Integrations

- @astrojs/tailwind - https://docs.astro.build/en/guides/integrations-guide/tailwind/
- @astrojs/sitemap - https://docs.astro.build/en/guides/integrations-guide/sitemap/
- @astrojs/mdx - https://docs.astro.build/en/guides/markdown-content/
- @astrojs/rss - https://docs.astro.build/en/guides/rss/

## 🚀 Project Structure

Inside of Dante Astro theme, you'll see the following folders and files:

```text
├── public/
├── src/
│   ├── components/
│   ├── content/
│   ├── data/
│   ├── icons/
│   ├── layouts/
│   ├── pages/
│   ├── styles/
│   └── utils/
├── astro.config.mjs
├── package.json
├── README.md
├── tailwind.config.cjs
└── tsconfig.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

There's nothing special about `src/components/`, but that's where we like to put any Astro (`.astro`) components.

The `src/content/` directory contains "collections" of related Markdown and MDX documents. Use `getCollection()` to retrieve posts from `src/content/blog/`, and type-check your frontmatter using an optional schema. See [Astro's Content Collections docs](https://docs.astro.build/en/guides/content-collections/) to learn more.

Any static assets, like images, can be placed in the `public/` directory.

## Astro.js Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## Want to learn more about Astro.js?

Check out [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).

## Credits

- Demo content generate with [Chat GPT](https://chat.openai.com/)
- Images for demo content from [Unsplash](https://unsplash.com/)

## License

Licensed under the [GPL-3.0](https://github.com/JustGoodUI/dante-astro-theme/blob/main/LICENSE) license.
