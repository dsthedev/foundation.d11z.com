# Changelog

## Version 0.0.3 (2019.12.30)

- Adds layout for 404 (also as an example for custom layouts)
- Adds 404 page content (used for .htaccess rule)
- Adds browserupgrade notice as a partial (also as an example)

## Version 0.0.2 (2019.12.30)

- Adds html5-boilerplate as dev dep for reference
- Pulls modified `.htaccess` file from `html5-boilerplate` into `src/`
- Disables open in `gulpfile.babel.js`
- Adds `apache()` function to gulp flow to copy `.htaccess` file alone during build process
- Adds `.vscode` to `.gitignore` because sftp config is in there!
- Adds `.code-workspace` file for easier project management within VSCode
- Adds `sherpaDirs()` function to `gulpfile.babel.js` to put styleguide in a "subfolder" (no .html extension!)
  - Also adds examples of adding new folders and/or styleguide files (to use for documentation maybe?)

## Version 0.0.1 (2019.12.30)

- Updates `readme.md` for use within this project's scope
- Updates `package.json` with this project's details
- Adds `TODO.md` to track desired internal tasks
- Deletes `yarn.lock` file, I've never used yarn for Foundation dev work
- Deletes `.bowerrc` file, I've never used bower for Foundation dev work
- Removes `.cache` & `.idea` from `.gitignore, not sure what they're from
- Formats most files with Prettier (`alt+shift+F`)

## Version 0.0.0 (2019.12.30)

- Used `foundation new --framework sites --template zurb` as starting point
- Initial Commit
