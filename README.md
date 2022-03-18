# React and webpack boilerplate

This is a simple template for starting a React app with webpack bundler.

## Table of contents

- [Setup](#setup)
- [Webpack Config](#webpack-config)
- [Babel JS](#babel-js)

## Setup

To start a React application using this template just:

1. Clone it.
2. Change the project name and description in the `package.json`
3. Set the title for your app in `public/index.html`
4. Install dependencies by running `npm install`

## Webpack config

This is divided in 3 files by using _webpack-merge_:

There is the `webpack.config.base.js` file, in which you will find the main settings that are the same both for development mode, and for production.

Also, there is the `webpack.config.dev.js` file, that adds some settings for the dev server. It's for development mode and you can run the server with this config by doing **npm start**. By default it is using the port 3006, but you can change that in this file, if you want to.

Finally, you have the `webpack.config.prod.js` file, that adds some optimizations for production mode. To use this config, you should run **npm run build**. This will create a `dist` folder (short for distribution) in the root directory, and inside the bundle of the project. Open the `index.html` file to check it out!

## Babel JS

Babel comes already installed and with a basic `.babelrc` config file. This will allow you to use all Javascript latest features by compiling the code and transforming it into code understandable by any browser.
