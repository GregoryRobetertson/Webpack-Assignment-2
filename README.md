# Webpack-Assignment-2

# Webpack Loaders and Plugins Assignment

## Objective
The objective of this assignment was to delve deeper into Webpack loaders and plugins. I aimed to configure Webpack to handle CSS files using `style-loader` and `css-loader`, ultimately optimizing the CSS output for production with the `MiniCssExtractPlugin`.

## Steps Taken

### Part 1: Project Setup

#### Initialize Project
1. Created a new directory named `webpack-loaders-plugins`.
2. Initialized a new npm project inside the directory using `npm init -y`.

#### Installed Dependencies
3. Installed Webpack, Webpack CLI, `style-loader`, and `css-loader` as development dependencies.

#### Project Structure
4. Created a `src` directory with `index.js` and `styles.css` files.
5. Established a `dist` directory containing an `index.html` file.

### Part 2: Configuring Loaders

#### Webpack Configuration
6. Crafted a `webpack.config.js` file, setting the entry point as `./src/index.js` and the output as `bundle.js` in the `dist` directory.

#### CSS Loaders
7. Incorporated a rule in `webpack.config.js` to employ `style-loader` and `css-loader` for `.css` files.

### Part 3: Implementing CSS

#### Adding CSS
8. Added custom CSS styles in `src/styles.css`.
9. Imported `styles.css` into `src/index.js`.

#### HTML Setup
10. Linked the bundled JavaScript file in `dist/index.html`.

### Part 4: Installing and Configuring MiniCssExtractPlugin

#### Installing the Plugin
11. Installed `mini-css-extract-plugin` as a development dependency.

#### Plugin Configuration
12. Updated `webpack.config.js` to utilize `MiniCssExtractPlugin` for extracting CSS into separate files.
13. Substituted `style-loader` with `MiniCssExtractPlugin.loader`.

### Part 5: Building for Production

#### Production Build
14. Added a script in `package.json` to facilitate a production build using Webpack (`"build": "webpack --mode=production"`).
15. Executed the build script to generate production files.

#### Testing the Build
16. Opened `dist/index.html` in a browser to verify that the external CSS file was loaded and applied correctly.

## Conclusion
In conclusion, through this assignment, I successfully configured Webpack loaders and plugins to handle CSS files, ensuring optimized production output.
