# foundation.d11z.com

[![devDependency Status](https://david-dm.org/zurb/foundation-zurb-template/dev-status.svg)](https://david-dm.org/zurb/foundation-zurb-template#info=devDependencies)

This is a personal exploration project using the [Foundation for Sites](http://foundation.zurb.com/sites) "ZURB" template for website development. It has a Gulp-powered build system with these features:

- Handlebars HTML templates with Panini
- Sass compilation and prefixing
- JavaScript module bundling with webpack
- Built-in BrowserSync server
- For production builds:
  - CSS compression
  - JavaScript module bundling with webpack
  - Image compression

## Installation

To work on this project, your computer needs:

- [NodeJS](https://nodejs.org/en/) (Version 11.15.0 or greater recommended, tested with 11.15.0)
- [Git](https://git-scm.com/)

```bash
cd path/to/projects
git clone https://github.com/dsthedev/foundation.d11z.com.git
cd foundation.d11z.com
npm install
```

**Notice:** The installation can take a while (5+ min) depending on your network / hardware.

## Development

```bash
cd path/to/foundation.d11z.com
npm start
```

To create compressed, production-ready assets, run `npm run build`.

## Publish

To publish this project to a live domain, I recommend using the SFTP plugin for Visual Studio Code to connect and sync files up. Example:

```json
[
  {
    "name": "Project Name",
    "ignore": [
      ".vscode",
      ".git",
      ".DS_Store",
      "cron",
      ".well-known",
      "cgi-bin",
      "docs",
      "fonts",
      "images",
      "swfs",
      "*.pem"
    ],
    "port": 21,
    "protocol": "sftp",
    "username": "user@sub.domain.com",
    "password": "****************", // Not recommended to keep this in, better to use ssh or enter manually (tedious but secure!)
    "context": "./dist/",
    "host": "sub.domain.com",
    "remotePath": "/",
    "downloadOnOpen": false,
    "uploadOnSave": true
  }
]
```

## Resources

- [NVM](https://github.com/nvm-sh/nvm) - I recommend using this to manage node / npm on your computer to easily switch versions in case a new version breaks something.
- [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) - Auto format most files with common standards
  - I recommend using `"editor.formatOnSave": true` for almost thought-free cleaner code
- [Add PrismJS to Foundation](https://www.dsthedev.com/configuration/add-prismjs-code-highlighting-to-foundation-for-sites/)

## Known Issues

- The use of triple-space in markdown files with sherpa doesn't match format standards.  If format on save is enabled it will strip them out and break the sticky sidebar nav