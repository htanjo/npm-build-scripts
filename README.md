# npm build scripts
> Simple build scripts for frontend development based on npm.

## Features
- [ESLint](http://eslint.org/)
- [Sass](http://sass-lang.com/) compiling
- [Autoprefixer](https://github.com/postcss/autoprefixer)
- [Browsersync](https://www.browsersync.io/) server
- Image optimization

## Getting started
1. Download **[package.json](https://github.com/htanjo/npm-build-scripts/raw/master/package.json)**.
2. Create **`app`** directory and place your web contents in it.

   ```
   your-project/
   ├── app/           : Static web contents
   └── package.json   : Download from this repository
   ```

3. Install dependencies.

   ```
   $ npm install
   ```

## Commands
- **`npm start`**  
  Start local development server.  
  During development, Sass compiler and ESLint will run automatically when you save a file.

- **`npm run build`**  
  Run ESLint, compile Sass to CSS and optimize images.

- **`npm run`**  
  Show all available tasks.

## License
Copyright (c) 2016 Hiroyuki Tanjo. Licensed under the [MIT License](LICENSE).
