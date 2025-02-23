# Vite + Deno

<img src="./public/vite-deno.svg" title="Vite + Vue + Deno"/>

This is an example repo of running Vite with Deno.

You can see live site at: https://vite-deno-example.deno.dev

This repo is based on a `deno-vue` template from `create-vite-extra`:

```
$ deno run -A --unstable npm:create-vite-extra --template deno-vue
```

## Notes

- You need to use `.mjs` or `.mts` extension for the `vite.config.[ext]` file.

## Papercuts

Currently there's a "papercut" for Deno users:

- peer dependencies need to be referenced in `vite.config.js` - in this example
  it is only `vue` package that needs to be referenced

## Running

You need to have Deno v1.25.4 or later intalled to run this repo.

Start a dev server:

```
$ deno task dev
```

## Deploy

Build production assets:

```
$ deno task build
```

This repository uses
[Deno Deploy and Git integration](https://deno.com/deploy/docs/projects#git-integration),
where deployment is happening as part of the CI pipeline.
