# DCI Boilerplate sass + parcel

An HTML CSS boilerplate with built-in sass support:

- Development server powered by [parcel](https://parceljs.org/) with sass compilation and auto-reload.
- Deployments to github pages with [gh-pages](https://www.npmjs.com/package/gh-pages)

## Get Started

- [Setup](#setup)
- [Useful Commands](#useful-commands)
- [Project Structure](#project-structure)
- [Credits](#credits)

## Setup

1. Clone this repository into a new project folder

2. Delete the boilerplate's git history to ensure that the project history only includes your commits

   ```
   cd <project folder>
   rm -rf .git
   ```

3. Edit `package.json` to add you project's name

   `package.json`

   ```json
   {
     "name": "[project name]",
     ...
     "author": "[your name]"
   }
   ```

4. Edit `src/index.html` to add your projects name

   ```html
   ...
   <head>
     ...
     <title>[project name]</title>
   </head>
   ...
   ```

5. Start a new git repository and make an initial commit. This will make sure that you can work on your project with git.

   ```
   git init
   git add . && git commit -m "Initial commit"
   ```

6. Install the dependencies

   ```
   npm install
   ```

7. Happy Coding!

## Useful Commands

### Development

Run **parcel-live-server** and start coding!

```
npm start
```

### Production

Compile source code from **src** and create an optimized production bundle in **dist** folder ready for **deployment**.

```
npm run build
```

### Deploy to Github Pages

Deploy your code to **Github Pages**: this script creates a 'gh-pages' branch and publishes the **dist** folder. For this to work, make sure you already have a remote repository on github.

```
npm run publish
```

## Project Structure

Any project created with this boilerplate will follow the structure below:

```
Project
│   README.md
│   package.json
|   package-lock.json
└───src
│   │   index.html
│   |   sassy-css.scss
|   └───images
└───dist
```

### `README.md`

The README should contain a brief description of your project, feel free to delete this guide or rename it to add your own description.

### `package.json` & `package-lock.json`

These files contain various information about you, your project and the project dependencies, as well as useful scripts to help you with the development process.

### `src` & `index.html`

The `src` folder contains any file you would want to add to your website. **This is the main folder you will be working in**.

`index.html` is the main page for your website which you will be working on. Feel free to add any new `html` pages you create directly in the `src` folder.

### `main.scss`

The `main.scss` file will contain any `scss` code you will be writing.

### `images`

Contains all images of your project

### `dist`

The `dist` folder will be automatically generated whenever your run the start or build script:

```bash
npm start
npm run build
```

`npm start` will create a non optimized bundle and `npm run build` will create an optimized production bundle, ready to be deployed. It is excluded from `git` tracking since it is not customary to include compiled code in a development project.
