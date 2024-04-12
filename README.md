Charity website template - ARCHIVED
Nice fluid website template, designed by cssauthor and coded by Maxim Orlov.

Demo: http://website-templates.github.io/charity_responsive-template

Mockup demo Product mockup created with http://frame.lab25.co.uk/

Contents
Folder and file structure
Requirements:
Editorconfig
How to start
Site configuration
Tasks
Cleanup
Dev
Build
Rebuild
Server
Sprite
Live reload
License
Folder and file structure
./
├── .editorconfig
├── Gruntfile.js
├── package.json
├── README.md
|
├── grunt_tasks/                               * grunt tasks
|   ├── config/                                * grunt tasks config
│   |   ├── paths.js
│   |   └── aliases.js
│   |
|   └── task.js
|
├── screenshots/                               * responsive test screenshots
|
├── dev/                                       * site source
│   ├── images/                                * image sources
|   │
│   ├── pug/                                   * templates
|   |   ├── blocks/                            * blocks library
|   │   |   └── block.pug
|   │   ├── helpers/                           * helper mixins
|   │   ├── vendor/                            * third-party code
|   │   ├── layouts/                           * page layouts
|   │   └── pages/                             * main pages templates
|   │
|   ├── stylus/                                * stylus preprocessor styles
|   |   ├── blocks/                            * blocks library
|   │   |   └── block.styl
|   │   ├── helpers/                           * mixins and vars
|   │   ├── vendor/                            * third-party code
|   │   ├── custom.styl
|   │   ├── noscript.styl
|   │   └── screen.styl
|   │
│   ├── helpers/                               * helper files
|   |   ├── favicon.ico
|   |   └── .htaccess
|   │
│   └── data/                                  * configs and data for templates
│
└── build/                                     * built source
    ├── index.html
    ├── page.html
    |
    └── static/                                * static assets
        ├── css/                               * minified styles
        |
        ├── images/                            * minified images
        |
        └── fonts/                             * @font-face-ready webfonts

Requirements
Node.js
Build sytem: Grunt or Gulp
Optionally:
Editorconfig
Ruby and Ruby Sass
Editorconfig
This project has an .editorconfig file at the root. It describes indent style, trailing whitespaces etc. See more details here

How to start
If you haven't used Grunt before, be sure to check out the Getting Started guide, as it explains how to use Gruntfile as well as install and use Grunt plugins.

Before start you need to have installed npm, grunt, ruby, and ruby-sass globallly.

A few simple steps to start:

Install dependencies from package.json by running: npm install.
Run tasks from the list below and start devevelopment!
Edit general settings in dev/data/config.json See Site configuration section
Site configuration
This boilerplate uses Pug templates with external data configs. Main settings can be found in dev/data/config.json file. And they're available for usage in templates with config.key-name

Tasks
Here comes groups of grunt tasks with some explanations

Cleanup
Remove placeholders from work directories. Grunt: grunt cleanup

Remove gitkeep files
Dev
Dev task with static server. Grunt: grunt dev

Compile Stylus stylesheets
Add vendor prefixes in css
Combine media queries in css files
Compile Pug templates
Sync helpers and other assets
Sync images
Run BrowserSync static server with live reload using
Watch for changes and run dev task
Build
Build task. Grunt: grunt build

Minify images
Minify stylesheets
Minify html
Run BrowserSync static server
Rebuild
Regenerate and build project by running all tasks. Grunt: grunt rebuild

Compile Stylus stylesheets
Add vendor prefixes in css
Combine media queries in css files
Compile Pug templates
Sync helpers and other assets
Sync images
Minify images
Minify stylesheets
Minify html
Server
Run server without watching for changes. Grunt: grunt server

Run BrowserSync static server
Live reload
This project uses BrowserSync as static server with enabled and configured live reload option.

License
MIT