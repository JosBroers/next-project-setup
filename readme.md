# Next project setup

## Prerequisites

Install the Node version listed in `.nvmrc` (use a Node version manager such
as [NVM for Mac](https://github.com/nvm-sh/nvm) or [NVM for Windows](https://github.com/coreybutler/nvm-windows))

## Environment Variables

In order to use Google Tag Manager and set the SEO defaults follow these steps:

1. Add the following three variables to Vercel:
   - `NEXT_PUBLIC_GTM` (Your Google Tag Manager ID, e.g. `GTM-ABCDE1F`)
   - `NEXT_PUBLIC_SITE_NAME` (Your site name, e.g. `Next.js Project Setup`)
   - `NEXT_PUBLIC_SITE_URL` (Your site URL, e.g. `https://next-project-setup.jobrodo.nl/`)
2. Install the Vercel CLI with `npm install -g vercel`
3. Connect your project to vercel with `vercel link` and configure credentials accordingly
4. Pull the environment variables with `vercel env pull`

## Scripts

- Use `yarn` or `yarn install` to install the dependencies
- Use `yarn ci` to remove the file `yarn.lock` and the directory `node_modules` and reinstall the dependencies
- Use `yarn dev` to start a local dev server at [http://localhost:3000](http://localhost:3000)
- To build the application for production, use `yarn build`
- To start a production server, use `yarn start`
- To export application as static HTML, use `next build && next export`
- For checking on unused imports, use `yarn find:unused`
- For analyzing the chunks and modules, use `yarn analyze`

## Vercel CLI

- To install Vercel CLI use `npm install -g vercel`
- To connect a project use `vercel link` and configure credentials accordingly
- Use `vercel env pull` to get the environment variables
- Use `vercel dev` to deploy a local test server at [http://localhost:3000](http://localhost:3000)
- Use `vercel` to deploy a preview build
- Use `vercel --prod` to deploy a production build

## Depcheck

- To install Depcheck use `npm install -g depcheck typescript`
- Use `depcheck` to analyze the dependencies in the project
