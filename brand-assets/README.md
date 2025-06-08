# Brand Assets

This folder contains files used to customize the NocoDB UI branding and its Open Graph meta tags. Replace the images in `./assets` with your own to change the look of the UI and previews.

The mapping of each file to its destination inside the project is stored in `assets.json`. During the local docker build the files listed in that mapping are copied into the NocoDB sources before the GUI build step.

Add your own versions of these files keeping the same names and formats. Dimensions of the original images are recorded in `assets.json` for reference.

The UI meta tags can be customized by setting these environment variables:

- `NC_BRAND_SITE_NAME`
- `NC_BRAND_TITLE`
- `NC_BRAND_DESCRIPTION`
- `NC_BRAND_URL`

See `docker-compose/2_pg_branded/docker-compose.yml` for an example of how to provide them when running with Docker Compose.
