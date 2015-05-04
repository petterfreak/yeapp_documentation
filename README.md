INTRODUCTION
================

### Thanks
Thank you for puchasing this framework. If you have any questions or suggestions do not hesitate to ask us!

### YeApp features
"YeApp" is a fully responsive admin web App built with AngularJS. This application is designed to robust/rich/large web applications. Flat,clean,dynamic,highly customizable.

- __Flat UI/UX__: inspirated by IOS & Apple
- __Responsive design__: Bootstrap 3 (Angular Bootstrap)
- __Powerful layout__: Box,Dock,Fold,Fix,Desktop... 
- __AngularJS__: plugins only in angular way 
- __Solid workflow__: Grunt tasks - Bower management
- __Built with LESS__: easy modification
- __Nested routing & views__: de-facto solution to flexible routing
- __Lazy loading__: load modules on demand
- __Internationalization__: 18n for your Angular apps
- __Dynamic breadcrumb__: itegrated to the ui.router 
- __3 runnable app__: Tasks, Documents, Mail
- __5 premade scheme__: you can build your own with LESS
- __Localstorage support__: save user settings in browser 
- __Angular modules__: many useful and popular modules
- __CSS helpers__: you can build unique widgets 
- __Unique ideas__: many handcrafted pages
- __Separetad files__: carefully designed app structure
- __Mobile states__: managed from Angular app
- __Onepage frontend theme__
- and much more...

### Getting Started

__File structure__

``` html
    >-- app/
    |   >-- dist/
    |   >-- dummy/
    |   >-- fonts/
    |   >-- icons/
    |   >-- img/
    |   >-- js/
    |   >-- lang/
    |   >-- scripts/
    |   |   >-- controllers/
    |   |   |   >-- main.js
    |   |   >-- directives/
    |   |   >-- filters/   
    |   |   >-- app.js 
    |   |   >-- app_constants.js
    |   |   >-- app_routes.js
    |   >-- styles/
    |   >-- views/
    |   >-- index.html
    >-- bower_components/
    >-- documentation/
    >-- frontend_onepage/
    >-- less/
    |   >-- app/
    |   |   >-- skins/
    |   |   >-- helpers/
    |   >-- bootstrap/
    |   >-- main.less
    |   >-- frontend_onepage.less
    >-- node_modules/ 
    >-- .bowerrc
    >-- Gruntfile.js
    >-- bower.js
    >-- package.js
```

__app/__ 
This folder contains the web-application files.

- __dist/__ Here you will find the concatenated JS files by grunt. (app.js & built.js)
- __dummy/__ This folder contains dummy json files for the demo pages
- __fonts/__ This folder contains fonts and their files
- __icons/__ This folder contains icons and their files
- __img/__ This folder contains the dummy images of the theme
- __js/__ Here you will find JS files that do not have bower package wrapper
- __lang/__ This folder contains language specific json files
- __scripts/__ Here you will find AngularJS files.
  - __controllers/__ contains the controllers of the app
    - __main.js__ root controller    
  - __directives/__ contains the directives of the app
  - __filters/__  contains the filters of the app
  - __app.js__ main root angular module and its dependency container (set config and run options)
  - __app_constants.js__ contains the lazy loading files structure of the app (angular modules,controllers,jquery...)
  - __app_routes.js__ contains the routes of the app (ui-router)
- __styles/__ Contains the static css files generated for the app (from less)
- __views/__ This folder contains the html and partial files for the views used for the app. 
- __index.html__ Main index.html (the app's entry point)

__bower_components/__ This folder contains the bower package files

__documentation/__ Here you will find the documentation of the template (You are reading now this)

__frontend_onepage/__ Here you will find the files of the frontend(onapage) template

__less/__ This folder contains the LESS files for the core styles and bootstrap styles.

  - __app/__ 
    contains the LESS source with the app components
  - __app/skins/__ 
    contains the skin's files and variables
  - __app/helpers/__ 
    contains the css helpers of the template
  - __bootstrap/__
    contains the LESS source files for Bootstrap
  - __main.less__
    less include file for the app (app + bootstrap less files)
  - __frontend_onepage.less__
    less include file for the frontend page (app + bootstrap less files)

__node_modules/__ This folder contains the node (npm) modules

__.bowerrc__ - Shows where the bower_components folder is

__Gruntfile.js__ - contains the grunt environment markup & tasks 

__bower.json__ - contains the bower packages list

__package.json__ - contains the list of the running environment necessary files,compilers (bower,grunt,less compiler)


### How to run it?
#### __1. First step: (install npm dependencies)__

You will need to install Node.js (http://nodejs.org/) on your computer.

If you have installed Node.js, you'll need to run a command in the project's root folder:
(Please note that any commands must be ran from the project's root folder.)

``` js
npm install
```

If you issue the above command, the dependencies will be installed in the root directory of your project __/node_modules/__. (grunt,bower,grunt tasks...) 

#### __2. Second step: (install javascript dependencies)__

``` js
bower install
```

If you issue the above command, the dependencies will be installed in the root directory of your project __/bower_components/__. (Angular/Jquery/3rd party modules/libs/frameworks) 

#### __3. Third step: (run)__

``` js
grunt serve
```

This command executes the Grunt's tasks (build:dev) and starts the web server where the application (will) run(s).
So this will start a local webserver and open up your default browser.

__Note: If you would like to use any other type of webserver (for example apache,tomcat) then you have to execute the "build:dev" or "build:dist" command. 
After these you can copy the "app" and "bower_components" directory into the webserver's www directory.__ <a href="#introduction-grunt">Here you can read more about the build procedure</a>


### NPM packages
__Npm packages (package.json)__
All npm packages contain a file, usually in the project root, called package.json - 
this file holds various metadata relevant to the project. This file is used to give 
information to npm that allows it to identify the project as well as handle the project's 
dependencies. It can also contain other metadata such as a project description, the version 
of the project in a particular distribution, license information, even configuration data - 
all of which can be vital to both npm and to the end users of the package.

### Bower
__Bower packages (bower.json)__
Web sites are made of lots of things & frameworks, libraries, assets, utilities, 
and rainbows. Bower manages all these things for you.

### Grunt
__Grunt markup file (Gruntfile.js)__
In one word: automation. The less work you have to do when performing repetitive
 tasks like minification, compilation, unit testing, linting, etc, the easier 
your job becomes. After you've configured it through a Gruntfile, a task runner 
can do most of that mundane work for you—and your team—with 
basically zero effort.

The Grunt ecosystem is huge and it's growing every day. With literally hundreds 
of plugins to choose from, you can use Grunt to automate just about anything 
with a minimum of effort. If someone hasn't already built what you need, 
authoring and publishing your own Grunt plugin to npm is a breeze.

If you haven't used Grunt before, be sure to check out the Getting Started guide, as it explains how to create a Gruntfile as well as install and use Grunt plugins.
http://gruntjs.com/getting-started

#### Grunt tasks

``` js
grunt serve
```
This command executes the Grunt's tasks (clean,less,cssmin,concat:libs,concat:angular,uglify,connect:livereload,watch) 
and starts the web server where the application (will) run(s). So this will start a local webserver and open up your default browser.

``` js
grunt watch
```

This watches files for changes and runs tasks based on the changed files after your browser will be refreshed automatically.

``` js
grunt clean
```

This command erases the cache files.

``` js
grunt concat:libs
```

This command concatenates the necessary & required files of the app into one file. (jquery, angularjs plugins & libs)


``` js
grunt concat:angular
```

This command concatenates the necessary & required files of the app into one file. (angularjs controllers,directives,routes,constants..)

``` js
grunt less
```

This command compiles the less files to css that the app use. (app/styles/result.css)


``` js
grunt cssmin
```

This command minifies the compiled css files of the app which was generated by the previous task (grunt less)

``` js
grunt uglify
```

This command minifies the concatenated js files of the app which was generated by the concat:angular and concat:libs.

``` js
grunt build:dev
```

This command executes the following commands: clean, less, concat:libs, concat:angular

``` js
grunt build:dist
```

This command executes the following commands: clean, less, concat:libs, concat:angular, cssmin, uglify.


### Less
Less is a CSS pre-processor, meaning that it extends the CSS language, 
adding features that allow variables, mixins, functions and many other 
techniques that allow you to make CSS that is more maintainable, themable 
and extendable.

Less runs inside Node, in the browser and inside Rhino. There are also many 3rd 
party tools that allow you to compile your files and watch for changes.

#### You can find YeApp's less files in the /less directory

- LESS files can easily be found because they are separated per component basis.
For example a table element specific less file can be found under the less/app/tables.less path.

- The less files of bootstrap are copied into under __/less/bootstrap__ path to avoid the conflict of different versions (during bower update).

- We strive for not modifying the Bootstrap's files directly. The bootstrap specific less files are overridden by the application what you can find under __less/app__ directory.

- The __less/main.less__ file stands for the includes of mandatory dependencies of the App.

- The __less/frontend_onepage.less__ stands for the includes of mandatory dependencies of the Frontend.

__Note: If you would like to create custom components, we strongly advise you that to put the new content into a different file, otherwise it will be overridden during the update.__



Main angular modules
================

### Angular Bootstrap
Bootstrap components written in pure AngularJS by the AngularUI Team

YeApp is using Angular bootstrap (ui and components)

documentation: https://angular-ui.github.io/bootstrap/

### OcLazyLoad
Load modules on demand (lazy load) in AngularJS

YeApp's constants of angular/js modules are placed in this file: __app/scripts/app_constants.js__

__ _REQUIRES__ - Jquery or core libraries and their assets

__ _MODULES__ - Angular's third party modules and/or wrappers 

__ _CONTROLLERS__ - YeApp's controllers and modules

Note: You can read more about these arrays <a href="#angularjs-add-new-libplugin">here</a>

documentation: https://github.com/ocombe/ocLazyLoad 

### UI Router
The de-facto solution to flexible routing with nested views

YeApp's routes are placed in the __app/scripts/app_routes.js__ file.

#### __Example of route config:__

``` js
    .state('components.sortable', {
        url: "/sortable",
        templateUrl: "views/ui-components/sortable.html",
        resolve: resolveRoute(['ng-nestable','ui.sortable'],['jquery.nestable','jquery-ui'])
    })
```

- While the app is running , files can be downloaded for the specific routes with the help of OcLazyLoad lib (on demand). Resolve property needs to be filled out in order to download files.  
resolveRoute() method helps you to create the resolve object by passing the name of the script what you want to load for the actual route.

#### Explanation of parameter signature of resolveRoute() method
- __first parameter : array__: the names of the angularJS/controller/module what you want to load from the __ _MODULES__ and __ _CONTROLLERS__ arrays.
- __second parameter : array__: the keys of the Jquery/3rd party file(s) what you want to load from __ _REQUIRES__ array.

Note: You can read more about these arrays <a href="#angularjs-add-new-libplugin">here</a>

Note: of course this method just an util, you can use the
OcLazyLoad's default load mechanism. documentation: https://github.com/ocombe/ocLazyLoad#works-well-with-your-router

documentation: https://github.com/angular-ui/ui-router


### UI Router breadcrumb

YeApp's ui-router is extended with ui-breadrcumb.

Angular-breadcrumb is a module for AngularJS, which generates a breadcrumb for any page of your application. It is strongly based on the ui-router framework and its hierarchical tree of states.

``` js
    .state('home', {
        url: '/home',
        templateUrl: 'views/home.html',
        controller: 'HomeCtrl',
        ncyBreadcrumb: {
            label: 'Home page' // angular-breadcrumb's configuration
        }
    })
```

documentation: https://github.com/ncuillery/angular-breadcrumb

### Internationalization

You can find the language specific json files in the: __app/lang/__ folder

angular-translate is an AngularJS module that makes your life much easier when it comes to i18n and l10n including lazy loading and pluralization.

documentation & usage: http://angular-translate.github.io/


CONTENT
================

### HTML structure

YeApp's main html DOM __app/index.html__

``` html
#Angular app declaration
<html ng-app="yeappApp">

  <head>
    #metas,css,fonts include
  </head>  

  #angular root controller to handle layout properties and some constant stuff
  <body ng-controller="MainCtrl">
    
    <div id="mainPreloaderHolder">
        #page load(angular) preloader content
    </div>

    #root holder
    <div class="mainApp">

        #header and view definiton for ui-router
        <div class="mainAppHeader" ui-view="mainHeader">
            #header content
        </div>

        #sidebar and view definiton for ui-router 
        <div class="mainAppAside" ui-view="mainSideBar">
            #sidebar content
        <div>

        #page views of routes
        <div class="mainAppContent" ui-view>
            #page content
        </div>

    </div>

    #toaster directive to notifications
    <toaster-container></toaster-container>

    #slidedown holder
    <div class="slideDownSection">
        #slidedown content
    </div>

    #scripts include

  </body>
</html>
```

### Sidebar

You can find here: __app/views/main-sidebar.html__

#### Simple sidebar item

``` html
<li ui-sref-active="active"> 
    <a ui-sref="dashboard">
        <i class="fa fa-dashboard"></i> 
        <div>
            <span >{{ 'DASHBOARD' | translate }}</span>
        </div>
    </a>
</li>
```

angular ui.router documentation: http://angular-ui.github.io/ui-router/site/#/api/ui.router.state.directive:ui-sref

#### Collapsible sidebar item

``` html
<li ng-class="{opened:$state.includes('ui')}">  
    <a collapse-menu>
        <i class="fa fa-star-o"></i> 
        <div>
            <span >{{ 'UI' | translate }}</span>
            <i class="nav-arrow fa fa-angle-right "></i>
        </div>
    </a>
    <ul class="nav nav-list nav-children main-nav">
        <li class="fold-header">
            <a>
                <div>
                    <span >{{ 'UI' | translate }}</span> 
                </div>
            </a>
        </li>
        <li  ui-sref-active="active" > 
            <a ui-sref="ui.general">
                <i class="fa fa-caret-right repl"></i> 
                <div>
                    <span >{{ 'GENERAL' | translate }}</span>
                </div>
            </a>
        </li>
        ...
    </ul>
</li>
```

- as you can see in the first line the "opened" class will be added into the li tag, if the $state variable contains the "ui" specific route
- $state variable is a global variable, it contains the information about the actual route's state.
- We created a useful directive called "collapse-menu" for you. It performs the collapse/drop-down feature of the sidebar.
- The first child of the collapsible list(nav-children) has to be a specific "fold-header" item. The child's content is the same as its parent's content.


### Header

You can find here: ___app/views/main-header.html__

- Two important 'main div-tag' can be found in the main-header.html
  - "__navbar-header__": this contains the logo and navbar for mobile(xs) view
  - "__navbar-collapse__": this contains the collapsible menu and navbar for desktop/tablet

### Views/Partials

The views can be found in the following directory: __/app/views/__

The views are separated per component basis to speed up the searches after them.
For example The html views of mailing service can be found in the following directory /app/views/mail



AngularJS
================

### Global app scope - Main.js 

Yeapp has a root controller which added into the body tag (MainCtrl). You can find the root controller here: __app/scripts/controllers/main.js__

The next steps will show you the methods/variables that contain the application. 
These methods and variables can be used anywhere in the angular's app. There are other methods and variables that can be used for the demo app.


#### $rootScope.getLayoutType() 

- If you call this method then you will get the resolution of the screen. (screen-xs,screen-sm,screen-md,screen-lg)

``` html
...
<body breakpoint="{0:'screen-xs', 768:'screen-sm', 992:'screen-md', 1200:'screen-lg'}">
...
```
- These breakpoints are placed in the body tag. Of course you can easily change them.

documentation: https://github.com/snapjay/angularjs-breakpoint



#### $rootScope.getDefaultSettings() 
- This method returns the array of the default settings for the app. The following will show you its structure:

``` js
{
    showSettingsBtn: true,
    settings: {
        theme: 'themeBlue',
        showSideBar: true,
        showApps: false,
        dockAside: false,
        boxedLayout: false,
        fixedHeader: true,
        fixedAside: false,
        desktopLayout: false,
        lang: 'en_US'
    },
    themes: [
        {
            name: 'blue theme',
            theme: 'themeBlue'
        },
        {
            name: 'grey theme',
            theme: 'themeGrey'
        },
        {
            name: 'yellow theme',
            theme: 'themeYellow'
        },
        {
            name: 'dark grey theme',
            theme: 'themeDarkGrey'
        },
        {
            name: 'neon green theme',
            theme: 'themeNeonGreen'
        }
    ]
}
```

   - __settings__: this contains the properties of the app. More information can be found about the layout: <a href="#layouts-classes">here</a>
   - __settings.theme__: actual theme's name
   - __settings.lang__: default language
   - __themes__: Color schemes which can be selected inside the demo app


#### $rootScope.setDesktopLayout()

This function provides the desktop (application) layout for the app. More information can be found about this: <a href="#layouts-desktopfixed-layout">HERE</a>


#### $rootScope.changeLanguage()

You can change the app's language in running time with this function.

#### $rootScope.mobileLayout:bool 

This variable contains true if the app is in mobile view. Otherwise its value is false.


### Add new lib/plugin

####__+Add new default plugin__

There is a possibility to define plugins and libraries which will be downloaded at the time of first page initialization
(Example: AngularJS,Jquery,Oclazyload...)

You can easily add files in the following file: 'Gruntfile.js'. Just add the paths of the files. 

__Jquery/Other 3rd party js files__: __concat.libs.src__
``` js
...
libs: {
    src: [
        'bower_components/jquery/dist/jquery.min.js',
    ...
]}
```

__AngularJS files: __concat.libs.angular__
``` js
...
angular: {
    src: [
        'app/scripts/app.js',
    ...
]}
```

__Note for CSS and other files: You have to register/include your own css and other custom asset files in the head of main index.html.__


####__+Add new lazyload plugin__

As it was mentioned previously, the files can be downloaded during running time. (on demand). You can easily add files here: __app/scripts/app_constants.js__


#### Jquery or other 3rd party files [_REQUIRES array]

``` js
 ...
 'moment': ['../bower_components/moment/min/moment.min.js', '../bower_components/moment/min/moment-with-locales.min.js']
 ...
```

#### Angular modules [_MODULES array]

``` js
 ...
{
    name: 'textAngular',
    files: ['../bower_components/textAngular/dist/textAngular-sanitize.min.js', '../bower_components/textAngular/dist/textAngular.min.js']
}
 ...
```

#### App controllers/modules [_CONTROLLERS array]

``` js
 ...
{
    name: 'App.mail',
    files: ['scripts/controllers/mail.js']
}
 ...
```

### Add new controller/view...

 If you need a new Controller, just create a file in the __/app/scripts/controllers/__ folder. After these, you do not forget to add it into the _CONTROLLERS array.

__Note: in OcLazyLoad every controller has to be wrapped by a module. Actually the files in the /app/scripts/controllers folder are controllers but its wrapped by a module__

 * __Controllers__ : __app/scripts/controllers__ folder

 * __Views__ : __app/views__ folder


### Custom directives

We made a few useful & unique directives for the app. __app/scripts/directives/directives.js__

#### __collapseMenu__  

It performs the collapse/drop-down feature of the sidebar.

``` html
<li>  
    <a collapse-menu>
        <i class="fa fa-star-o"></i> 
        <div>
            <span >{{ 'UI' | translate }}</span>
            <i class="nav-arrow fa fa-angle-right "></i>
        </div>
    </a>
    <ul class="nav nav-list nav-children main-nav">
    ...
    </ul>
</li>

```

#### __sparkLine__  

Angular directive for jquery's sparkline.

``` html
<spark-line data="sparkline.data" options="sparkline.options"></spark-line>
```

Parameters:

 - data
 - options

http://omnipotent.net/jquery.sparkline/#s-about

#### __morris__  

Angular directive for morris chart

``` html
<div id="morris4" morris type="'donut'" options="morris.donut" ></div>
```

Parameters:

 - type: area,bar,line,donut
 - options: http://morrisjs.github.io/morris.js/

#### __iCheck__  

Angular directive for iCheck

http://fronteed.com/iCheck/

``` html
<label class="icheck"><input type="checkbox" i-check ng-model="test"> Option one </label>
```

#### __resizeBrowser__ 

This directive added into a body tag. It detects the browser resize and then broadcasts an event.

Event's name: resizeBrowser

``` html
...
<html ng-app="yeappApp" resize-browser>
...
```

``` js
...
    scope.$on('resizeBrowser', function (e) {
        render();
    });
...
```

#### __focusMe__

This is the directive is used if the given variable(focus-me property) is true, then the focus is moving to that element.

``` html
<input type="text" class="form-control" placeholder="What needs to be done?" ng-model="newTodo.text" focus-me="list.addMode">
```

#### __vectorMap__ 

Angular directive for Jquery's vectormap

``` html
<div vector-map options="mapOptions" width="'auto'" height="300" class="m-10"></div>
```

Parameters:

 - options
 - width
 - height


LAYOUTS
================

### Classes

Layout can be changed via the following classes applied to the body tag

 * __closed-folded-sidebar__ : Condenses the sidebar showing only icons (in mobile(xs) the sidebar is hidden)

 * __show-sidebar__ : The sidebar is forced to showing all item

 * __fixed-aside__ : The sidebar become fixed

 * __dock-aside__ : The sidebar become horizontal 

 * __fixed-header__ : The header become fixed

 * __desktop-layout__ : The layout become fixed while the user can scroll only content

if you want the __boxed layout__, you have to add the __'container' class__ to the __'mainApp' section__ 


### Basic Layout

If you want to use the basic scrolled layout then you do not have do anything.

### Desktop/Fixed Layout

- If the desktop layout is needed to be used, in your controller you have to call the setDesktopLayout() method with true value.
Also, you need to be sign up for the destroy event and the method with false value need to be added, in order to go back to the default layout.

- This method adds the "desktop-layout" class to the body tag.


``` js
    ...
    $scope.setDesktopLayout(true);

    $scope.$on("$destroy", function handler() {
        $scope.setDesktopLayout(false);
    });
    ...
```

Variation of layout samples can be found in the next folder: __app/views/starters__

Note: This layout cannot be seen in a Mobile resolution.


THEME COLORS
================

### Less

YeApp creates color variations with the help of Less. These files can be found in the next folder: __less/app/skins__
These are separated by different files for user friendly purpose. 

The skin generator can be found in this file: __less/app/theme-generator.less__

### Create custom skin/theme

#### __1. step (create skin/theme file)__

A new file needs to be created in the __less/app/skins__ folder by calling it with the new skin's name

#### __2. step (write the content)__
For example: __less/skins/blue.less__

``` js

.themeDefs(1){
    @themeName:themeBlue;

    @themeBgColor:#ddeefb;

    @listItemHoverColor: transparent;

    @themeBorderRight: 1px solid #bad0df;
    @themeBorderBottom: #a5c6df;

    @themeFontColor: #454648;
    @themeFontHoverColor: #007aff;

    @themeItemActiveBgColor: #cae8fb;
    @themeItemActiveFontColor: #007aff;

    @listItemBorderTopColor: #e4f2fc;
    @listItemBorderBottomColor: #cde3f1;

    @listItemActiveBorderTopColor: #b1dbf9;
    @listItemActiveBorderBottomColor: #b1dbf9;
}

```

 * __.themeDefs(1)__ - in a new theme file you must increase the value in the themeDefs

 * __@themeName__ - the name of the new theme

 * __@themeBgColor__ - background-color of the sidebar

 * __@listItemHoverColor__ - background-color of the hovered item of the sidebar

 * __@themeBorderRight__ - border-right of the sidebar

 * __@themeBorderBottom__ - border-bottom color of the navbar-brand

 * __@themeFontColor__ - deafult font color of the sidebar

 * __@themeFontHoverColor__ - default font hover color of the sidebar

 * __@themeItemActiveBgColor__ - active item background-color of the sidebar

 * __@themeItemActiveFontColor__ - font color of the active item of the sidebar

 * __@listItemBorderTopColor__ - border top color of the item of the sidebar

 * __@listItemBorderBottomColor__ - border bottom color of the item of the sidebar

 * __@listItemActiveBorderTopColor__ - border top color of the active item of the sidebar

 * __@listItemActiveBorderBottomColor__ - border bottom color of the active item of the sidebar

#### __3. step (include the new file)__

The newly created file needs to be included in this file: __less/main.less__

#### __4. step (increase the index of the loop)__

- The value of __@numberOfThemes__ needs to be increased by one, in this file: __less/app/theme-generator.less__

__Note: If a unique CSS is needed in your color scheme, then first a variable is needed to be created, this variable will be essential to use in the other schemes too.
After this, it needs to be written in the "theme-genarator.less" file, within inside the buldThemes() method that where these properties are located in the DOM tree.__

HELPERS
================

### Css helpers

__Note:__

- If the numbers are shown in the "Other options" column, it means the numbers can be changed in the name of the class (unit: pixel)
- If the coma separates the list of classes, CSS rule applies to both (alias)

#### Padding

| Class | CSS          | Other options          |
| ------------- | ----------- | ----------- |
| no-p,no-padding | padding:0px | |
| no-p-i | padding:0px !important | |
| no-p-b | padding-bottom:0px !important | |
| no-p-t | padding-top:0px !important | |
| no-p-l | padding-left:0px !important | |
| no-p-r | padding-right:0px !important | |
| no-p-t-b,no-p-b-t | padding-top:0px !important & padding-bottom:0px !important | |
| no-p-r-l,no-p-l-r | padding-right:0px !important & padding-left:0px !important | |
| p-3 | padding:3px | 5-10-15-20-30-50 | 
| p-3-i | padding:3px !important | 5-10-15-20-30-50 |
| p-t-3 | padding-top:3px !important | 5-10-15-20-30-50 |
| p-b-3 | padding-bottom:3px !important | 5-10-15-20-30-50 |
| p-r-3 | padding-right:3px !important | 5-10-15-20-30-50 |
| p-l-3 | padding-left:3px !important | 5-10-15-20-30-50 |
| p-t-b-3,p-b-t-3 | padding-top:3px !important & padding-bottom:3px !important | 5-10-15-20-30-50 |
| p-r-l-3,p-l-r-3 | padding-right:3px !important & padding-left:3px !important | 5-10-15-20-30-50 |

#### Margin

| Class | CSS          | Other options          |
| ------------- | ----------- | ----------- |
| no-m,no-margin | margin:0px | |
| no-m-i | margin:0px !important | |
| no-m-b | margin-bottom:0px !important | |
| no-m-t | margin-top:0px !important | |
| no-m-l | margin-left:0px !important | |
| no-m-r | margin-right:0px !important | |
| no-m-t-b,no-m-b-t | margin-top:0px !important & margin-bottom:0px !important | |
| no-m-r-l,no-m-l-r | margin-right:0px !important & margin-left:0px !important | |
| m-3 | margin:3px | 5-10-15-20-30-50 | 
| m-3-i | margin:3px !important | 5-10-15-20-30-50 |
| m-t-3 | margin-top:3px !important | 5-10-15-20-30-50 |
| m-b-3 | margin-bottom:3px !important | 5-10-15-20-30-50 |
| m-r-3 | margin-right:3px !important | 5-10-15-20-30-50 |
| m-l-3 | margin-left:3px !important | 5-10-15-20-30-50 |
| m-t-b-3,p-b-t-3 | margin-top:3px !important & margin-bottom:3px !important | 5-10-15-20-30-50 |
| m-r-l-3,p-l-r-3 | margin-right:3px !important & margin-left:3px !important | 5-10-15-20-30-50 |

#### Border separators for UI

| Class | CSS          | Other options          |
| ------------- | ----------- | ----------- | |
| box-border-r,b-b-r | border-right:1px solid #c1c1c1 !important | |
| box-border-l,b-b-l | border-left:1px solid #c1c1c1 !important | |
| box-border-t,b-b-t | border-top:1px solid #c1c1c1 !important | | 
| box-border-b,b-b-b | border-bottom:1px solid #c1c1c1 !important | | 
| box-border-r-light,b-b-r-l | border-right:1px solid #d9d9d9 !important | |
| box-border-l-light,b-b-l-l | border-left:1px solid #d9d9d9 !important | |
| box-border-t-light,b-b-t-l | border-top:1px solid #d9d9d9 !important | |
| box-border-b-light,b-b-b-l | border-bottom:1px solid #d9d9d9 !important | &nbsp; |

- These specific classes will help to separate the panels and boxes.

#### Borders

| Class | CSS          | Other options           |
| ------------- | ----------- | ----------- | |
| b-panel | border: 1px solid #d9d9d9 |  |
| b-solid | border-style:solid |  |
| b-dashed | border-style:dashed |  |
| b-dotted | border-style:dotted |  |
| b-1px | border-width:1px | 2-3-4-5 |
| b-lt | border-color:#ddd |  |
| no-border,no-b | border-color: transparent;border: none; | |
| no-border-i,no-b-i| border-color: transparent !important;border: none !important; | |
| no-b-t | border-top:none !important |  |
| no-b-r | border-right:none !important |  |
| no-b-l | border-left:none !important |  |
| no-b-b | border-bottom:none !important | &nbsp; |
| b-primary | border-color: primary | &nbsp; |
| b-success | border-color: success | &nbsp; |
| b-info | border-color: info | &nbsp; |
| b-warning | border-color: warning | &nbsp; |
| b-danger | border-color: danger | &nbsp; |

#### Border radius

| Class | CSS          | Other options           |
| ------------- | ----------- | ----------- | |
| no-b-rad     | .border-radius(0px,0px,0px,0px)| |
| no-b-rad-i    | .border-radius(0px,0px,0px,0px) !important     | |
| b-rad-3 | .border-radius(3px,3px,3px,3px) | 3-15-30-100-200-500 | 
| b-rad-r-l-3,b-rad-l-r | .border-radius(0px,0px,3px,3px) | 6-15-30-100-200-500 | 
| b-rad-t-b-3,b-rad-b-t | .border-radius(0px,0px,3px,3px) | 6-15-30-100-200-500 | 

#### Background & colors

| Name | Optional classes          |
| ------------- | ----------- |
| bg-primary | lt + dk |
| bg-info | lt + dk     |
| bg-success | lt + dk     |
| bg-warning| lt + dk      |
| bg-light | lt + dk      |
| bg-dark | lt + dk     |
| bg-dark | lt + dk     |
| bg-black |  lt + dk    |
| bg-danger | lt + dk     |

* lt class = lighter
* dk class = darker

#### Grid & gutter

Columns create gutters (gaps between column content) via padding. That padding is offset in rows for the first and last column via negative margin on .rows.
documentation: http://getbootstrap.com/css/#grid

| Class | Description          |
| ------------- | ----------- |
| row-gap-5      | gutter - 5px |
| row-gap-10     | gutter - 10px    |
| row-panel-10 | panel - margin bottom: 10px  |

#### Position

| Class | Description          | Options          |
| ------------- | ----------- | ----------- | |
| item      | parent |  |
| wrapper     | child    | top,bottom,left,right |

Usage:

``` html
<div class="item" style="height:500px;">
    Content
    <div class="wrapper top right">
        Im in the top right
    </div>
    <div class="wrapper bottom left">
        Im in the bottom left
    </div>
</div>
```

#### Table layout

| Name | Description          | Comment          |
| ------------- | ----------- | ----------- | |
| r-sm-table     | display:table  |  |
| col-sm-cell,c-sm-cell |  display:table-cell   | &nbsp;  |
| v-middle |  vertical-align: middle   | &nbsp;  |
| v-top |  vertical-align: top   | &nbsp;  |
| v-bottom |  vertical-align: bottom   | &nbsp;  |

This layout cannot be seen in a Mobil version 

CREDITS
================

### AngularJS

#### Main files
 * AngularJS (sanitize,resource,route,cookies,animate,touch,translate) https://angularjs.org/
 * angular-bootstrap https://angular-ui.github.io/bootstrap/
 * angular-ui-router https://github.com/angular-ui/ui-router
 * oclazyload https://github.com/ocombe/ocLazyLoad
 * angular-breadcrumb https://github.com/ncuillery/angular-breadcrumb
 * ngStorage https://github.com/gsklee/ngStorage
 * ngprogress http://victorbjelkholm.github.io/ngProgress/
 * angularjs-breakpoint https://github.com/snapjay/angularjs-breakpoint
 * angular-ui-switch https://github.com/xpepermint/angular-ui-switch
 * angular-datepicker https://github.com/alongubkin/angular-datepicker
 * bootstrap-daterangepicker https://github.com/dangrossman/bootstrap-daterangepicker
 * ng-bs-daterangepicker https://github.com/luisfarzati/ng-bs-daterangepicker
 * AngularJS-Toaster https://github.com/jirikavi/AngularJS-Toaster
 * angular-aside https://github.com/dbtek/angular-aside
 * angular-slimscroll https://github.com/ziscloud/angular-slimscroll
 * angular-ui-select https://github.com/angular-ui/ui-select
 * angular-translate-loader-url https://github.com/angular-translate/bower-angular-translate-loader-url
 * angular-translate-loader-static-files https://github.com/angular-translate/bower-angular-translate-loader-static-files
 * ng-focus-on https://github.com/goodeggs/ng-focus-on
 * angular-loading-bar: http://chieffancypants.github.io/angular-loading-bar/


#### Lazy load files
 * angularMoment https://github.com/urish/angular-moment
 * NgSwitchery https://github.com/servergrove/NgSwitchery
 * ui.sortable https://github.com/angular-ui/ui-sortable
 * textAngular https://github.com/fraywing/textAngular
 * angularUnderscoe https://github.com/floydsoft/angular-underscore
 * ng-chartjs https://github.com/petermelias/angular-chartjs
 * angular-rickshaw https://github.com/ngyewch/angular-rickshaw
 * angular-flot http://github.com/develersrl/angular-flot
 * easypiechart http://rendro.github.io/easy-pie-chart/
 * angular-ui-calendar http://angular-ui.github.io/ui-calendar/
 * angular-validator https://github.com/kelp404/angular-validator"
 * angular-file-upload https://github.com/nervgh/angular-file-upload
 * angular-wizard https://github.com/mgonto/angular-wizard
 * angular-xeditable http://vitalets.github.io/angular-xeditable 
 * ng-table https://github.com/esvit/ng-tabl
 * angular-bootstrap-slider http://seiyria.github.io/bootstrap-slider/
 * ng-bootbox https://github.com/eriktufvesson/ngbootbox
 * angular-bootstrap-nav-tree https://github.com/nickperkinslondon/angular-bootstrap-nav-tree
 * angular-native-picker https://github.com/alongubkin/angular-datepicker
 * ngImgCrop https://github.com/alexk111/ngImgCrop
 * ng-nestable http://kamilkp.github.io/ng-nestable
 * angular-ui-utils https://github.com/angular-ui/ui-utils
 * AngularGM https://github.com/dylanfprice/angular-gm-bower
 * angular-ui-grid http://ui-grid.info
 * angular-masonry https://github.com/passy/angular-masonry
 * ui.bootstrap.datetimepicker http://dalelotts.github.io/angular-bootstrap-datetimepicker
 * ng-grid-panel https://github.com/Hacklone/ng-grid-panel
 * ng-nvd3 https://github.com/sattarab/ng-nvd3/
 * angularjs-slider https://github.com/PopSugar/angular-slider
 * ngAutocomplete https://github.com/wpalahnuk/ngAutocomplete
 * Smart Table http://lorenzofox3.github.io/smart-table-website/
 * SweetAlert https://github.com/oitozero/ngSweetAlert
 
### JQuery & others

#### Main files
 * Jquery https://jquery.com/
 * Bootstrap http://getbootstrap.com/
 * Moment http://momentjs.com/
 * iCheck http://fronteed.com/iCheck/
 * flot http://www.flotcharts.org/
 * slimScroll http://rocha.la/jQuery-slimScroll

#### Lazy load files
 * jquery-ui https://jqueryui.com/
 * underscore http://underscorejs.org/
 * switchery http://abpetkov.github.io/switchery/
 * fullcalendar http://fullcalendar.io/ 
 * Chart.js http://www.chartjs.org/
 * rickshaw http://code.shutterstock.com/rickshaw/
 * d3 http://d3js.org/ 
 * nvd3 http://nvd3.org/
 * sparkline http://omnipotent.net/jquery.sparkline/
 * raphael http://raphaeljs.com/
 * morris.js http://morrisjs.github.io/morris.js/
 * bootbox http://bootboxjs.com/
 * jquery.nestable http://dbushell.github.io/Nestable/
 * masonry http://masonry.desandro.com/
 * imagesloaded https://github.com/desandro/imagesloaded
 * seiyria-bootstrap-slider https://github.com/seiyria/bootstrap-slider
 * jquery-jvectormap http://jvectormap.com/
 * FooTable https://github.com/fooplugins/FooTable

#### Fonts/Icons
 * Font Awesome http://fortawesome.github.io/Font-Awesome/
 * Linea http://linea.io/
 * Open sans https://www.google.com/fonts/specimen/Open+Sans


UPGRADING
================
We offer free support and updates to our valuable customers!

SUPPORT
================
You can request for support via themeforest comments.

We will assist you any problem you face while buidling your app via YeApp framework.
