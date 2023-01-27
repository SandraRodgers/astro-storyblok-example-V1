# Astro Storyblok Example

This example uses Astro version 1.9.2 with Storyblok. It's in SSR mode.

To set this up so Netlify deploys changes to this repo, do the following:

- Add a new site to Netlify. Select "Import an existing project"
- Connect to Github and choose the repo you want to deploy

To make the publish command work in Storyblok so that the site builds, do the following:

- Go into Netlify, choose the site, then go to `Site Settings`
- Go into the `Build and Deploy` Settings
- Find the `Build Hooks` section. Create a new build hook. Name it what you want, then copy the key.
- Go into your Storyblok space. Go to `Settings`.
- Go into Webhooks and add the key where it says `Story published & unpublished`

Now when you make a change in Storyblok, you can click `publish` and the change will cause the Netlify site to rebuild with that change.

To see the site in the Storyblok editor, and to see the Visual Editor working:
- Go into Storyblok `Settings` for the project, then `Visual Editor`
- Add the Netlify url for you site where it says `Location (default environment)`
