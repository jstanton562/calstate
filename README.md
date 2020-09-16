# Installation

Calstate is a subtheme of the Radix base Drupal theme. It uses [Webpack](https://webpack.js.org) to compile and bundle SASS and JS. It is built to run on Drupal 8.x -- It can be used on Drupal 9.x by installing the dev version of Radix, but it may require some tweaking.

#### Step 1
Install and enable [Radix 8.x-4.x and Components](https://www.drupal.org/project/radix) in your Drupal project

#### Step 2
Place the Calstate subtheme in the following location: *docroot/themes/custom/calstate*

#### Step 3
In your Drupal site's admin interface install the Calstate theme and set as default

#### Step 4
Make sure you have [Node and npm installed](https://docs.npmjs.com/getting-started/installing-node). 
Go to the root of the Calstate directory and run the following command: `npm install` 

#### Step 5
Update the `proxy` variable in *webpack.mix.js*.

#### Step 6
In your Drupal site's admin interface, set up the initial Block layout as follows:
1. Navbar branding
	* Site branding
2. Navbar left
	* Main navigation
3. Navbar right
	* Search
4. Header
	* Status messages
	* Tabs
5. Content
	* Page title
	* Main page content
6. Sidebar
7. Footer
	* Footer menu
8. Subfooter
	* User account menu
	* Help
	* Primary admin actions

#### Styling and Templating
* Regions are defined in the calstate.info.yml file
* Most project specific styles and behaviors can be written in the *assets/css/project.style.css* and *assets/js/project.script.js* files
* CSU styles have been built into the SASS here: *src/sass*, primarily in the *base* directory
* Run one of the following commands from the Calstate root to compile the SASS: `npm run watch` (to watch for changes), `npm run dev`, or `npm run production` 
* The Google fonts reference is located in the *templates/html.html.twig* file
* Turn on Twig Debug mode in *docroot/sites/default/services.yml* (around line 58) to identify which templates are being used
