# Docker Image for NextJS

⚡️ For apps running Next.JS that want the fastest possible build time ⚡️

## Features

- 🏔 Build on the [node:alpine](https://hub.docker.com/_/node) flavor, a trusted & well-maintained base image
- 🌩 Installs with [pnpm](https://pnpm.io/) using the [fetch](https://pnpm.io/cli/fetch) protocol, much faster than `pnpm install` for docker builds
- 📦 Builds into a [standalone build](https://nextjs.org/docs/advanced-features/output-file-tracing), ultimately shipping smaller code to the container

## Usage

- Copy the `Dockerfile` into your existing Next.JS app
- Add `{'output': 'standalone'}` to your `next.config.js` file
    - See `Dockerfile:28` for more details on if you should opt-out of this behavior

```js
    export.module = {
        'output': 'standalone',
        ...otherConfig
    }
```


## Contributing

PRs are always welcome

## License

> MIT License
