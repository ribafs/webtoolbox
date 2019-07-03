# The Web Toolbox
_A collection of handy, free-to-use tools for web developers, programmers and designers alike._

Inspired by _thetoolbox.cc_ that went offline some time ago.

## Adding new tools or making fixes
Please see [contributing.md](https://github.com/ToshNeox/webtoolbox/blob/master/CONTRIBUTING.md).

## Developing locally
The application is developed and built for production using the amazing [Parcel bundler](https://github.com/parcel-bundler/parcel).

Just clone the project locally, install dependencies with `npm i` and run `parcel index.html`.

Parcel will build the project and create a local development server at `http://localhost:1234` (if that port is available.)

### Updating the online site
The site is hosted using GitHub pages, serving content from the `gh-pages` branch.

This branch is a sub-tree of the master branch, using files from the `dist` folder on master.

To update the branch:

- Build the project using `parcel build index.html --public-url .`
- Commit the new site contents
- Update the branch using `git subtree push --prefix dist origin gh-pages`

The site should update as soon as GitHub Pages deploys from the new code.