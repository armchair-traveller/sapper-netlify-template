# Sapper Netlify Template

A minimal template for deploying Sapper to Netlify.

**Changes from Sapper default Rollup template**

Removals:

- Unnecessary routes like the blog and about page
  - Nav component
- Favicon and logo placeholder assets from both static folder and manifest
- Cypress testing folder and commands
- `_error.svelte` 404 route, doesn't work with export/Netlify anyway - [more info](https://github.com/sveltejs/sapper/issues/557)

Additions:

- build command exports then moves to `public` folder
- `netlify.toml` with functions activated, Node set to latest version, and using `public` folder to deploy
- .gitignore additions to account for these changes
- CSS border-box reset, I use this too much

The template is meant to be a structure like starting a Gatsby project blank. You have the folders but you should add everything else based on your needs.
Not every app needs a nav, favicon, etc. and this makes starting easier (once you're at least familiar with the folder structure of Sapper)

- To familiarize yourself with Sapper's folder structure and inner workings, the standard Sapper template can be referenced. This template is meant to get started quickly for pre-existing Sapper and Netlify users.
