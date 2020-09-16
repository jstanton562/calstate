# Installation

CALSTATE is a subtheme of the Radix base Drupal theme. It is built to run on Drupal 8.x. It can be used on Drupal 9.x by installing the dev version of Radix, but it may require some tweaking.

### Step 1
Install and enable [Radix and Components](https://www.drupal.org/project/radix) in your Drupal project






CALSTATE theme uses [Webpack](https://webpack.js.org) to compile and bundle SASS and JS.

#### Step 1
Make sure you have Node and npm installed. 
You can read a guide on how to install node here: https://docs.npmjs.com/getting-started/installing-node

If you prefer to use [Yarn](https://yarnpkg.com) instead of npm, install Yarn by following the guide [here](https://yarnpkg.com/docs/install).

#### Step 2
Go to the root of RADIX_SUBTHEME_NAME theme and run the following commands: `npm install` or `yarn install`.

#### Step 3
Update `proxy` in **webpack.mix.json**.

#### Step 4
Run the following command to compile Sass and watch for changes: `npm run watch` or `yarn watch`.
