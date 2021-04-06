# DHS Style Guide
Jekyll site for establishing the Department of Homeland Security Style Guide, based on the USWDS framework.

## Running code locally

All instructions for this respository have been created and tested using Mac OS. Due to certain server limitations, the top navigation (`_includes/site-nav.html`) and left navigation (`_layouts/content--sidebar.html`) have absolute links, instead of relative links to the pages.

After cloning the repo, navigate to the correct folder and install USWDS, Jekyll, and any necessary dependencies using:
```
npm start
```
Then, to run the site locally:
```
npm run serve
```
If all goes well, visit the site at http://localhost:4000.

USWDS assets are in `assets/uswds/fonts` and `assets/uswds/img`.

SASS files are kept in the `/_sass` directory. To override styles on a theme-level that will impact the entire site, edit `_uswds-theme-overrides.scss`. For specific components, USWDS will only accept USWDS color tokens. To use specific, DHS-branded colors that are not part of the USWDS theme, you will need to add custom styling in `_uswds-custom-styles.scss`. To create custom components based off the USWDS components, add new styles to `_custom-components.scss`.

To watch for changes and recompile the styles, run:
```
npm run watch
```
