INTRODUCTION
================

### Thanks
Thank you for purchasing. If you have any question or idea do not hesitate to ask us!

### YeApp features
"YeApp" is a fully responsive admin web App built with AngularJS. It use 
LESS CSS which makes it easy to modify.

- AngularJS
- 
...

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
    |   |   >-- directives/
    |   |   >-- directives/   
    |   |   >-- app.js 
    |   |   >-- app_constants.js
    |   |   >-- app_routes.js
    |   >-- styles/
    |   >-- views/
    >-- bower_components/
    >-- documentation/
    >-- frontend_onepage/
    >-- less/
    |   >-- app/
    |   |   >-- themes/
    |   |   >-- helpers/
    |   >-- bootstrap/
    |   >-- main.less
    |   >-- frontend_onepage.less
    >-- node_modules/ 
    >-- Gruntfile.js
    >-- bower.js
    >-- package.js
```

__app/__ folder
 - This folder contains the web-application files.

- __dist/__
Here you will find the concatenated JS files by grunt. (app.js & built.js)

- __dummy/__
This folder contains dummy json files for the demo pages

- __fonts/__
This folder contains fonts and their files

- __icons/__
This folder contains icons and their files

- __img/__
This folder the theme images (dummy)

- __js/__
Here you will find JS files that do not have bower package wrapper

- __lang/__
This folder contains the json files use for translation.

- __scripts/__
Here you will find AngularJS files.
  - __controllers/__ 
    contains the controllers of the app
  - __directives/__
    contains the directives of the app
  - __filters/__
    contains the filters of the app
  - __app.js__
    main root angular module and its dependency container (set config and run options)
  - __app_constants.js__
    contains the lazy loading files structure of the app (angular modules,controllers,jquery libs..etc)
  - __app_routes.js__
    contains the routes of the app (ui-router)

- __styles/__
Contains the static css files generated for the app (from less)

- __views/__
This folder contains the html and partial files for the views used for the app. 

__bower_components/__ folder - This folder contains the bower package files

__less/__ folder - This folder contains the LESS files for the core styles and bootstrap styles.

  - __app/__ 
    contains the LESS source with the app components
  - __app/themes__ 
    contains the theme files and variables
  - __app/helpers__ 
    contains the theme css helpers
  - __bootstrap/__
    contains the LESS source files for Bootstrap
  - __main.less__
    less include file for the app (app + bootstrap less files)
  - __frontend_onepage.less__
    less include file for the frontend page (app + bootstrap less files)

__node_modules/__ folder - This folder contains the node (npm) modules

__Gruntfile.js__ - contains the grunt environment markup & tasks 

__bower.json__ - contains the bower packages list

__package.json__ - contains the list of the running environment necessary files,compilers (bower,grunt,less compiler)


### How to run it?
__1. First step: (prepare)__

You will need to have installed Node.js (http://nodejs.org/) on your computer.

If you have installed Node.js, you'll need to run a command in the project's root folder:
(Please note that any commands must be ran from the project's root folder.)

``` js
npm install
```

If you issue the following command the dependencies will be installed in the root directory of your project. (grunt,bower,grunt tasks...) 

__2. Second step: (install javascript dependencies)__

``` js
bower install
```

If you issue the following command the dependencies will be installed in the root directory of your project. (bower/js/angular JS components) 

__3. Third step: (run)__

``` js
grunt serve
```

This command executes the Grunt's tasks and starts the nodejs server where the application (will) run(s).
So this will start a local webserver and open up your default browser.



### NPM packages
__Npm packages (package.json)__
All npm packages contain a file, usually in the project root, called package.json - 
this file holds various metadata relevant to the project. This file is used to give 
information to npm that allows it to identify the project as well as handle the project's 
dependencies. It can also contain other metadata such as a project description, the version 
of the project in a particular distribution, license information, even configuration data - 
all of which can be vital to both npm and to the end users of the package.

``` js
{
  "name": "yeapp",
  "version": "1.0.0",
  "dependencies": {
    "bower": "*",
    "git": "*",
    "grunt": "^0.4.5",
    "grunt-autoprefixer": "^0.7.3",
    "grunt-concurrent": "^0.5.0",
    "grunt-contrib-clean": "^0.5.0",
    "grunt-contrib-concat": "^0.4.0",
    "grunt-contrib-connect": "^0.7.1",
    "grunt-contrib-copy": "^0.5.0",
    "grunt-contrib-cssmin": "^0.9.0",
    "grunt-contrib-jshint": "^0.10.0",
    "grunt-contrib-less": "*",
    "grunt-contrib-uglify": "^0.4.0",
    "grunt-contrib-watch": "*",
    "grunt-filerev": "^0.2.1",
    "grunt-google-cdn": "^0.4.0",
    "grunt-newer": "^0.7.0",
    "grunt-ng-annotate": "^0.3.0",
    "grunt-svgmin": "^0.4.0",
    "grunt-usemin": "^2.6.2",
    "grunt-wiredep": "^2.0.0",
    "jshint-stylish": "^0.2.0",
    "load-grunt-tasks": "*",
    "time-grunt": "^0.3.1"
  },
  "engines": {
    "node": ">=0.10.0"
  },
  "scripts": {
    "test": "grunt test"
  }
}
```

### Bower
__Bower packages (bower.json)__
Web sites are made of lots of things & frameworks, libraries, assets, utilities, 
and rainbows. Bower manages all these things for you.

``` js
{
  "name": "yeapp",
  "version": "0.0.0",
  "dependencies": {
    "angular": "~1.3.8",
    "json3": "~3.3.1",
    "es5-shim": "~3.1.0",
    "bootstrap": "~3.2.0",
    "angular-resource": "~1.3.3",
    "angular-cookies": "~1.3.3",
    "angular-sanitize": "~1.3.3",
    "angular-animate": "~1.3.3",
    "angular-touch": "~1.3.3",
    "angular-route": "~1.3.3",
    "angular-moment": "~0.8.2",
    "angular-motion": "~0.3.3",
    "angularjs-breakpoint": "*",
    "d3": "~3.4.11",
    "nvd3": "~1.1.15-beta",
    "angularjs-nvd3-directives": "~0.0.7",
    "angular-masonry": "~0.10.0",
    "iCheck": "~1.0.2",
    "angular-ui-tree": "~2.1.5",
    "jquery-ui": "~1.11.1",
    "angular-ui-sortable": "~0.12.11",
    "fullcalendar": "~2.1.1",
    "angular-flot": "~0.0.6",
    "flot": "~0.8.3",
    "angular-rickshaw": "~0.3.0",
    "ng-chartjs": "~0.0.5",
    "oclazyload": "~0.5.0",
    "sparkline": "~2.1.2",
    "jquery.sparkline": "~2.1.2",
    "morris.js": "~0.5.1",
    "raphael": "~2.1.2",
    "jquery.easy-pie-chart": "~2.1.4",
    "angular-ui-switch": "~0.0.3",
    "angular-validator": "~0.2.5",
    "ngstorage": "~0.3.0",
    "angular-datepicker": "~1.0.3",
    "angular-file-upload": "~1.1.1",
    "angular-xeditable": "~0.1.8",
    "angular-wizard": "~0.4.0",
    "underscore": "~1.7.0",
    "ng-table": "~0.3.3",
    "AngularJS-Toaster": "~0.4.8",
    "angular-slider": "~0.2.3",
    "angular-aside": "~1.1.0",
    "bootbox": "~4.3.0",
    "angular-bootstrap-nav-tree": "*",
    "angular-native-picker": "~1.0.4",
    "ngImgCrop": "~0.2.0",
    "ng-nestable": "~0.0.1",
    "nestable2": "~1.2.2",
    "angular-ui-calendar": "~0.8.1",
    "jquery": "~2.1.1",
    "angular-ui-utils": "~0.1.1",
    "ng-focus-on": "~0.2.2",
    "chartjs": "~0.2.0",
    "flot.tooltip": "~0.8.4",
    "AngularGM": "~1.0.0",
    "angular-ui-grid": "~3.0.0-rc.16",
    "masonry": "~3.1.5",
    "imagesloaded": "~3.1.8",
    "angular-bootstrap-datetimepicker": "~0.3.7",
    "angular-breadcrumb": "~0.3.2",
    "slimScroll": "~1.3.3",
    "angular-slimscroll": "~1.1.2",
    "angular-translate": "~2.4.2",
    "angular-translate-loader-url": "~2.4.2",
    "angular-translate-loader-static-files": "*",
    "ui-select": "*",
    "angular-ui-select": "~0.9.6",
    "ng-grid-panel": "~0.1.0",
    "angular-bootstrap-slider": "~0.0.8",
    "seiyria-bootstrap-slider": "~3.1.0",
    "ngprogress": "~1.0.7",
    "bootstrap-daterangepicker": "~1.3.17",
    "textAngular": "~1.2.2",
    "ng-nvd3": "~0.0.2",
    "angularjs-slider": "~0.1.6",
    "ng-bs-daterangepicker": "~0.0.3"
  },
  "resolutions": {
    "angular": "~1.3.x",
    "jquery": "~2.1.x",
    "bootstrap": "~3.x",
    "es5-shim": "~4.1.x",
    "d3": "~3.4.x",
    "jquery-ui": "~1.11.x",
    "fullcalendar": "~2.1.x",
    "angular-translate": "~2.5.x"
  },
  "devDependencies": {
    "angular-mocks": "~1.2.0",
    "angular-scenario": "~1.2.0"
  },
  "appPath": "app"
}
```


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

__Grunt commands:__

``` js
grunt serve
```
This command executes the Grunt's tasks and starts the nodejs server where the application (will) run(s).
So this will start a local webserver and open up your default browser.

``` js
grunt watch
```

This command watches the changes of the files of the app (/app folder). If they changed, it executes the
following commands, after these your app in the browser automatically refresh.

``` js
grunt clean
```

This command empties the cache files.

``` js
grunt concat:libs
```

This command concatenates the necessary & required files of the app to one file. (jquery, angularjs plugins & libs)


``` js
grunt concat:angular
```

This command concatenates the necessary & required files of the app to one file. (angularjs controllers,directives,routes,constants..)

``` js
grunt cssmin
```

This command minifies the compiled css files of the app

``` js
grunt uglify
```

This command minifies the concatenated js files of the app


### Less
Less is a CSS pre-processor, meaning that it extends the CSS language, 
adding features that allow variables, mixins, functions and many other 
techniques that allow you to make CSS that is more maintainable, themable 
and extendable.

Less runs inside Node, in the browser and inside Rhino. There are also many 3rd 
party tools that allow you to compile your files and watch for changes.

``` js
grunt less
```

This command compiles the less files to css that the app use. (app/styles/result.css)


CONTENT
================

### HTML structure

YeApp's html main structure

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

        #header holder with angular controller
        <div class="mainAppHeader" ng-controller="AppheaderCtrl">
            #header content
        </div>

        #sidebar holder with angular controller and ui-router view definiton
        <div class="mainAppAside" ng-controller="AppsidebarCtrl" ui-view="mainSideBar">
            #sidebar content
        <div>

        #page views of routes
        <div class="mainAppContent" ui-view>
            #page content
        </div>

        #toaster directive to notifications
        <toaster-container></toaster-container>
        
        #slidedown holder
        <div class="slideDownSection">
            #slidedown content
        </div>

        #scripts include

    </div>

  </body>
</html>
```

### Sidebar

 - you can find here: ___app/views/main-sidebar.html__

#### Main sidebar structure

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
- you can find this sctructure in the angular ui.router documentation 
http://angular-ui.github.io/ui-router/site/#/api/ui.router.state.directive:ui-sref

#### Collapse item

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
    </ul>
</li>
```

- as you can see the first line, you can define "ng-class" property here to detect this
is collapsible item
- $state is a global variable that contains the current tree items of the route. So this example shows if the $state include the "ui" word add the 'opened' class to li tag 
- the collapse "a" html tag has a "collapse-menu" directive. It perform the collapse meachnism (open & close).
- the child ul's first li has to be a "fold-header", this tag is a fixed layout helper for the sidebar. (same as the parent collapse item)


ide kell egy snippet hogyan kell letrehozni egy sidebar itemet

### Header

- you can find here: ___app/views/main-header.html__

#### Main header html

- there is 2 holder div
  - "__navbar-header__": this contains the logo & navbar for mobile(xs) view
  - "__navbar-collapse__": this contains the collapsible menu (separeted to 2 section)



AngularJS
================

### Angular Bootstrap
Bootstrap components written in pure AngularJS by the AngularUI Team

YeApp is using Angular bootstrap (ui and components)

documentation: https://angular-ui.github.io/bootstrap/

### OcLazyLoad
Load modules on demand (lazy load) in AngularJS

YeApp angular/js modules constants in the __app/scripts/app_constants.js__

__ _REQUIRES__ - jquery or core libraries and their assets

__ _MODULES__ - angular third party modules and/or wrappers 

__ _CONTROLLERS__ - YeApp controllers (Notice: in oclazyload every controller is a module)

documentation: https://github.com/ocombe/ocLazyLoad 

### UI Router
The de-facto solution to flexible routing with nested views

YeApp routes are in the __app/scripts/app_routes.js__

__Example:__

``` js
    .state('components.sortable', {
        url: "/sortable",
        templateUrl: "views/ui-components/sortable.html",
        resolve: resolveRoute(['ng-nestable','ui.sortable'],['jquery.nestable','jquery-ui'])
    })
```

resolveRoute fgv egy seged fuggveny, hogy kevesebb koddal tudd betolteni a kivant js fileokat.
Elso parametere (array): betolteni kivant angularJS/controllers/modules from _MODULES and _CONTROLLERS
Second parameter: array of Jquery/3rd party libs from _REQUIRES

resolveRoute() method helps you to not use the oclazyload's difficult mechanism. 
resolveRoute() has 2 parameter. First parameter: array of angularJS/controllers/modules from _MODULES and _CONTROLLERS
Second parameter: array of Jquery/3rd party libs from _REQUIRES

documentation: https://github.com/angular-ui/ui-router

### UI Router breadcrumb

YeApp ui-router is extended with ui-breadrcumb.

documentation: https://github.com/ncuillery/angular-breadcrumb

### Internationalization

documentation: https://docs.angularjs.org/guide/i18n

### + Add new lib/plugin

####__+ Add new default plugin__

There is a possibility to define plugins and libraries which will be downloaded at the time of first page initialization
(Example: AngularJS,Jquery,Oclazyload...)

You can easily add files in the following file
Konnyeden hozzaadhatsz ilyen js fajlokat:
'Gruntfile.js' fajlban a 'concat/libs/src' reszben bekell jegyezned az eleresi utvonalat egy tomb elemkent

__Note for CSS and other files __: You have to register/include your own css and other custom asset files in the head of main index.html.

####__+Add new lazyload plugin__

If you want to load files in run time, you have to define these files in the OcLazyLoad's section arrays.  __app/scripts/app_constants.js__

- Jquery or other 3rd party files (__ _REQUIRES__)
``` js
 ...
 'moment': ['../bower_components/moment/min/moment.min.js', '../bower_components/moment/min/moment-with-locales.min.js']
 ...
```

- Angular modules (__ _MODULES__)
``` js
 ...
{
    name: 'textAngular',
    files: ['../bower_components/textAngular/dist/textAngular-sanitize.min.js', '../bower_components/textAngular/dist/textAngular.min.js']
}
 ...
```

- App controllers/modules (__ _CONTROLLERS__)
``` js
 ...
{
    name: 'App.mail',
    files: ['scripts/controllers/mail.js']
}
 ...
```


Ha futasi idoben akarsz betolteni fajlokat, akkor azokat elsonek bekell jegyezned az OcLazyLoad szekcioban felsorolt require tombokbe

### +Add new controller/view

 * __Controllers__ : __app/scripts/controllers__ folder

 * __Views__ : __app/views__ folder

### Custom directives

Keszitettunk par egyedi direktivat a theme-hez.

#### Directives (app/scripts/directives/directives.js)
 * __collapseMenu__ ez manageli a sidebar menu lenyilo mechanizmusat
 * __sparkLine__ sparkline jquery chart-hoz direktiva
 * __morris__ morris chart-hoz direktiva
 * __iCheck__ icheck pluginhoz direktiva
 * __resizeBrowser__ ez a direktiva, ha bejegyezed propertykent barmelyik tagbe, akkor browser resize eseten broadcastolja az esemeny bekovetkeztet
 * __vectorMap__ jquery vectormap direktivaja


### root Controller - Main.js 

As you can see in the content section, YeApp has a root controller that helps you to define methods,variables 
that you can reach in every child controllers & views.
__YeApp's global variables and methods:__

Mint ahogyan lathattod a struktura reszben, YeApp-ban van egy root controllere (MainCtrl), ami seged controllerkent viselkedik.
Ide akar bejegyezhetsz konstansokat,fuggvenyeket amiket elakarsz erni barmelyik gyerek controllerben.
Itt lathatod a mi altalunk megadott, demohoz hasznalt fuggvenyeket, valtozokat



LAYOUTS
================

### Classes

Layout can be changed via the following classed applied to the body tag

 * __closed-folded-sidebar__ : Condenses the sidebar showing only icons (in mobile(xs) view the sidebar is hidden)

 * __show-sidebar__ : The sidebar is forced to showing all item

 * __fixed-aside__ : The sidebar become fixed

 * __dock-aside__ : The sidebar become horizontal 

 * __fixed-header__ : The header become fixed

 * __desktop-layout__ : The layout become fixed while the user can scroll only content

if you want the __boxed layout__, you have to add the __'container' class__ to the __'mainApp' section__ 

in the __body__ tag there is a __'breakpoint' directive__ : you can change the view breakpoints, illetve ezeket hasznalthatod angularjs controllereken belul, hogy
a webapp tudja, eppen melyik view-ban van

### Basic Layout

If you want to use the basic scrolled layout, you dont have do anything

### Desktop Layout

If you want to use the desktop (boxed) layout, in your angular controller
you have to call the root controller's (MainCtrl) method, and you have to 
change false when you changed the route (subscribe to the destroy event
in your controller and set false the desktop layout)

``` js
    $scope.setDesktopLayout(true);

    $scope.$on("$destroy", function handler() {
        $scope.setDesktopLayout(false);
    });
```

This function adds the desktop layout class to the body tag


THEME COLORS
================

### Less
Yeapp less segitsegevel allitja ossze az egyes theme szinkombinaciokat.
A themek fajljait megtalahatod a __less/app/themes__ konyvtarba. Itt kulon fajlokra vannak bontva a theme scheme-k.
A theme szinkombinaciok generalasa a __less/app/theme-generator.less__ fajlban tortenik

### Create custom theme

#### __1. step (create theme file)__

themes mappaba keszits egy fajlt, az uj theme nevevel.

#### __2. step (write the content)__
Peldakent a blue.less fajl tartalma:

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

 * __.themeDefs(1)__ -  in a new file you must increment the value (az uj ertek mindig egyel nagyobbnak kell lennie mint az osszes theme osszege)

 * __@themeName__ - the theme's name (szokoz nem megengedett!)

 * __@themeBgColor__ - sidebar background color

 * __@listItemHoverColor__ - sidebar hover bg color

 * __@themeBorderRight__ - sidebar's right side separator border

 * __@themeBorderBottom__ - navbar-brand ???

 * __@themeFontColor__ - sidebar's deafult font color

 * __@themeFontHoverColor__ - sidebar's default font hover color

 * __@themeItemActiveBgColor__ - sidebar's active item bg color

 * __@themeItemActiveFontColor__ - sidebar's active item font color

 * __@listItemBorderTopColor__ - sidebar's item border top color

 * __@listItemBorderBottomColor__ - sidebar's item border bottom color

 * __@listItemActiveBorderTopColor__ - sidebar's active item border top color

 * __@listItemActiveBorderBottomColor__ - sidebar's active item border bottom color

#### __3. step (bejegyezni az theme fajlt)__

Az uj fajlt a less/main.less fajl-ban be kell includolni

#### __4. step (megnovelni a loop indexet)__

Megkell novelned a __less/app/theme-generator.less__ a __@numberOfThemes__ erteket eggyel


 * __Note__: ha barmilyen egyedi css-t akarsz berakni egy theme-be, csak jegyezd be egy less valtozokent, azonban figyelj arra, hogy ezt a variable-t a tobbi theme-ben is bekell jegyezned.
Ezek utan mar csak bekell irnod a 'theme-genarator.less' fajlban, a buldThemes() fuggvenyen belul, hogy ezek az uj css tulajdonsagok hol helyezkedjenek el a DOM tree-ben.



HELPERS
================

### Css helpers

#### Padding & Margin

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
| p-t-b-3,p-b-t-3 | padding-top:3px !important & padding-bottom:3px !important | 5-10-15-20-30-50
| p-r-l-3,p-l-r-3 | padding-right:3px !important & padding-left:3px !important | 5-10-15-20-30-50

 * Ezek a classok ervenyes a margin-okra is, csak kikell cserelni a p betut m-re

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
| box-border-b-light,b-b-b-l | border-bottom:1px solid #d9d9d9 !important | |

#### Borders

| Class | CSS          | Other options           |
| ------------- | ----------- | ----------- | |
| b-panel | border: 1px solid #d9d9d9 |  |
| b-solid | border-style:solid |  |
| b-dashed | border-style:dashed |  |
| b-dotted | border-style:dotted |  |
| b-1px | border-width:1px | 2-3-4-5 |
| b-lt | border-color:#ddd |  |
| no-b-t | border-top:none !important |  |
| no-b-r | border-right:none !important |  |
| no-b-l | border-left:none !important |  |
| no-b-b | border-bottom:none !important |  |

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

| Class | Description          |
| ------------- | ----------- |
| row-gap-5      | gutter - 5px |
| row-gap-10     | gutter - 10px    |
| row-panel-10 | panel - margin bottom: 10px  |

#### Position

absolut pozicionalashoz egy section-on belul

| Class | Description          | Options          |
| ------------- | ----------- | ----------- | |
| item      | parent |  |
| wrapper     | child, amire akarod a pozicionalast    | top,bottom,left,right |

#### Table layout

Ezek a classok mobil nezet kivetelevel az osszes resolutionben mukodnek

| Name | Description          | Comment          |
| ------------- | ----------- | ----------- | |
| r-sm-table     | table display |  |
| col-sm-cell,c-sm-cell |  table-cell display  |  |

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

UPGRADING
================
We offer free support and updates to our lovely customers!

SUPPORT
================
You can request for support via themeforest comments

We will assist you any problem you face while buidling your app via YeApp framework.
