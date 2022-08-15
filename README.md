## THE SDSS subtheme HAS MOVED

- The SDSS subtheme has been moved.
- This repo and site is now essentially outdated and defunct.
- The new repo is [SU-SWS/sdss_profile](https://github.com/SU-SWS/sdss_profile).
- 08/15/2022

# [Stanford SDSS](https://github.com/SU-SWS/sdss_subtheme)
##### Version: 9.x-1.0-dev

Changelog: [Changelog.txt](CHANGELOG.txt)

Description
---

Stanford SDSS is a Stanford subtheme that works with the Stanford Basic theme.

Documentation
---
See subtheming guides and best practices here:
https://devguide.sites.stanford.edu/front-end/drupal/sub-themes

Installation
---
1. Review the documentation link above for best practices, particularly the Do's and Don't's sections.
2. Add any specific brand colors you need (in addition to the decanter colors that are already available) to src/scss/utilities/variables/_colors.scss.
See all the colors already available through decanter: https://decanter.stanford.edu/page/brand-design-elements-color/
3. If desired, add font settings if you need to override and use fonts other than decanter fonts ( https://decanter.stanford.edu/page/brand-design-elements-typography/ ) [link],
by defining a font library in the themename.libraries.yml file.
4. If desired, add button mixins in src/scss/utilities/mixins/_buttons.scss with your button styles and then reference them and use them in src/scss/theme/_button.scss.
5. If desired, add cta and link mixins in src/scss/utilities/mixins/_cta.scss with your button styles and then reference them and use them in src/scss/theme/_cta.scss.
6. If you want to skin or theme a component, like a paragraph, create a _mycomponent.scss file in src/scss/components folder. Consider using a subfolder like 'cards' or 'banners' if applicable.

Configuration
---

Nothing special needed. Install, enable, and set as the default active theme.

Developer
---

If you wish to develop on this theme you will most likely need to compile some new css. Please use the sass structure provided and compile with the sass compiler packaged in this theme. To install:

```
npm install
```
After you've made a change you want to see processed, you can run:
```
npm run publish
```
This will process scss, js, and asset files, preparing them from the src directory to the dist directory.
It will also copy decanter twig templates from node_modules to the dist/templates/decanter directory to be used.

Contribution / Collaboration
---

You are welcome to contribute functionality, bug fixes, or documentation to this theme. If you would like to suggest a fix or new functionality you may add a new issue to the GitHub issue queue or you may fork this repository and submit a pull request. For more help please see [GitHub's article on fork, branch, and pull requests](https://help.github.com/articles/using-pull-requests)
