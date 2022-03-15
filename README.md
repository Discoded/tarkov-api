# The Hideout API 💻

[![deploy](https://github.com/the-hideout/tarkov-data-api/actions/workflows/deploy.yml/badge.svg)](https://github.com/the-hideout/tarkov-data-api/actions/workflows/deploy.yml)

This is the main API for [thehideout.io](https://thehideout.io/).

It's a simple [GraphQL](https://graphql.org/) API running on [Cloudflare workers](https://workers.cloudflare.com/).

This API powers all of thehideout.io and other notable projects as well:

- [ratscanner](https://github.com/RatScanner/RatScanner)
- [errbot](https://github.com/GrantBirki/errbot)
- [thehideout](https://play.google.com/store/apps/details?id=com.austinhodak.thehideout&hl=en_US&gl=US)

## API Playground 🎾

There is a GraphQL playground for you to use and test out

**Link:** [api.thehideout.io/___graphql](https://api.thehideout.io/___graphql)

Example Query:

```graphql
query {
  itemsByType(type: any) {
      id
      name
      shortName
      wikiLink
      iconLink
      updated
  }
}
```

> More examples can be found in our [graphql example docs](./docs/graphql-examples.md) 📚

## Development 🔨

- Start the dev environment by running `npm run dev`
- Then open up the playground on [localhost:8787/___graphql](http://127.0.0.1:8787/___graphql)

## Deployment 🚀

```bash
wrangler publish
```
