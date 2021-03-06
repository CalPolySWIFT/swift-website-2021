# Website

This website is built using [Docusaurus 2](https://v2.docusaurus.io/), a modern static website generator.

## Automated Deployment

When this respository receives a push (`git push`), it triggers a GitHub Action that deploys the website onto the `gh-pages` branch, where the GitHub Pages site is being hosted on. 

It takes around 1 minute and 15 seconds for the GitHub Action to complete, so keep this in mind when viewing the updated website.

Please use the Wiki for further documentation.

## Manual Deployment

### Installation

```
yarn install
```

The `yarn install` command will install all packages using the Yarn package manager.

### Local Development

```console
yarn start
```

This command starts a local development server and open up a browser window. Most changes are reflected live without having to restart the server.

### Build

```console
yarn build
```

This command generates static content into the `build` directory and can be served using any static contents hosting service.

### Deployment

```console
GIT_USER=<Your GitHub username> USE_SSH=true yarn deploy
```

If you are using GitHub pages for hosting, this command is a convenient way to build the website and push to the `gh-pages` branch.
