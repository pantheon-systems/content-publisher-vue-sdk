# Pantheon Content Publisher for Vue

A Vue SDK and Nuxt starter kits for building sites on [Pantheon Content Publisher](https://docs.content.pantheon.io). Use them as a reference when integrating Content Publisher with Vue or Nuxt.

> [!WARNING]
> This repository is archived and unsupported. It receives no bug fixes or security updates. Treat it as reference code rather than something to install as-is. The supported SDKs live in [content-publisher-sdk](https://github.com/pantheon-systems/content-publisher-sdk).

## What's here

### `packages/vue-sdk`

The `@pantheon-systems/pcc-vue-sdk` package, built on `@pantheon-systems/pcc-sdk-core`:

- **Vue plugin:** `pccPlugin` configures the Content Publisher client for the app.
- **Composables:** `useArticle` and `useArticles` fetch content reactively.
- **Article rendering:** `<ArticleRenderer />` turns Content Publisher article data into Vue elements, with default styles and support for smart components.
- **Live preview:** a preview indicator component for articles opened from the editor.
- **Nuxt integration:** `NuxtPantheonAPI` mounts the Content Publisher API handler (preview, publishing hooks, smart component discovery) as a Nuxt server route.

See [`packages/vue-sdk/README.md`](packages/vue-sdk/README.md) for setup and usage.

### `starters/vue-starter` and `starters/vue-starter-ts`

Complete Nuxt 3 sites in JavaScript and TypeScript, styled with Tailwind. Each one includes:

- Paginated article listing and article pages
- Server API routes that proxy Content Publisher
- Live preview
- An example smart component (`LeadCapture`)
