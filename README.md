# npm build scripts
> Simple build scripts for frontend development based on npm.

## Features
- **[Browsersync](https://www.browsersync.io/)** : Keep multiple browsers & devices in sync when building websites.
- **[Imagemin](https://github.com/imagemin/imagemin)** : Minify images: JPEG, PNG, GIF and SVG.
- **[ESLint](http://eslint.org/)** : Lint ECMAScript/JavaScript code.
- **[Sass](http://sass-lang.com/)** : Compile Sass stylesheets to CSS.
- **[Autoprefixer](https://github.com/postcss/autoprefixer)** : Add vendor prefixes to CSS rules.

## Downloads
|                     | Mini     | +Lint    | +Styles  | Full     |
|--------------------:|:--------:|:--------:|:--------:|:--------:|
| Browsersync         | ✔       | ✔       | ✔       | ✔       |
| Imagemin            | ✔       | ✔       | ✔       | ✔       |
| ESLint              | -        | ✔       | -        | ✔       |
| Sass & Autoprefixer | -        | -        | ✔       | ✔       |
|                     | **[Download][mini]** | **[Download][lint]** | **[Download][styles]** | **[Download][full]** |

## How to use
1. Download **package.json** from above.
2. Create **`public`** directory and place your web contents in it.

   ```
   your-project/
   ├── public/        : Static web contents
   └── package.json   : Download from this repository
   ```

3. Install dependencies.

   ```
   $ npm install
   ```

4. Start development.

   ```
   $ npm start
   ```

### Sass coding
If you want to code stylesheets in Sass, just create Sass files in `public`.  
CSS will be generated in the same folder.

```
public/index.scss
public/assets/styles/main.scss
public/assets/styles/_partial.scss     # Partial will not be generated to a CSS file
 ↓
public/index.css
public/assets/styles/main.css
```

## Commands
- **`npm start`**  
  Start local development server.  
  During development, Sass compiler and ESLint will run automatically when you save a file.

- **`npm run build`**  
  Run ESLint, compile Sass to CSS and optimize images.

- **`npm run`**  
  Show all available tasks.
  See [npm-run-script document](https://docs.npmjs.com/cli/run-script) for more details.

## License
Copyright (c) 2016 Hiroyuki Tanjo. Licensed under the [MIT License](LICENSE).

[mini]: downloads/mini/package.json?raw=true
[lint]: downloads/lint/package.json?raw=true
[styles]: downloads/styles/package.json?raw=true
[full]: downloads/full/package.json?raw=true
