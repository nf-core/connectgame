# nf-core/connectgame

Open-source Match-3 game done in PixiJS. The goal of this project is to provide a simple and comprehensive example of professional game development using PixiJS technologies.

This project is built on top of the following PixiJS-based libraries:

-   [PixiJS](https://github.com/pixijs/pixijs) A rendering library built for the web.
-   [PixiJS Sound](https://github.com/pixijs/sound) A WebAudio API playback library, with filters.
-   [PixiJS UI](https://github.com/pixijs/ui) For commonly used UI components in PixiJS.
-   [PixiJS AssetPack](https://github.com/pixijs/assetpack) Compile and optimise assets for the web.
-   [PixiJS Spine](https://github.com/pixijs/spine) Spine animation support for PixiJS

# License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).

## GSAP

This game uses GSAP for its animations. You can use the free version of GSAP for some commercial projects. However please check the licensing options from [GreenSock](https://greensock.com/licensing/).

# Features

-   A simple Match-3 game with special powers and effects
-   Basic navigation system to organise screens and popups
-   Asset loading management using PixiJS assets bundles
-   Persistent user settings for sound volume and game mode
-   Save & load scores and best scores
-   Animations, transitions and visual effects
-   Desktop & mobile compatible

# Prerequisites

-   NodeJS - https://nodejs.org/
-   NPM - Comes with NodeJS, for package management

# Setup & Run The Game

```sh
# Clone the repository
git clone https://github.com/maxulysse/connectgame

# Enter the project folder
cd ./connectgame/connectgame

# Install dependencies
npm install

# Start the project for development
npm run start
```

# Building The Game

```sh
# Compile the game for publishing, outputs to `dist/`
npm run build

# Build the game for publishing and preview it locally
npm run preview
```

# Compiling Assets

Assets are compiled whenever you start or build the project, but they are not 'watched' (yet) like regular code while developing. If you add/modify/remove any assets while developing, you have to run `npm run assets` manually to recompile them and make the changes to take effect.

# Project Structure

### `./src/main.ts` file

Where everything starts. Sets up the PixiJS app and initialise navigation.

### `./src/screens` folder

All screens displayed by the app.

### `./src/popups` folder

Modal panels that shows up on top of screens.

### `./src/match3` folder

The game itself, with all Match-3 related code featuring gameplay logic and piece visuals.

### `./src/ui` folder

All UI components shared across screens.

### `./src/utils` folder

All the shared utility code.

### `./raw-assets` folder

Uncompiled assets grouped in folders that will be translated into assets bundles for loading.