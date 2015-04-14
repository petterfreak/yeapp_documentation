INTRODUCTION
================

### Thanks
Thank you for purchasing. If you have any questions or suggestions do not hesitate to ask us!

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

__app/__ 
This folder contains the web-application files.

- __dist/__
Here you will find the concatenated JS files by grunt. (app.js & built.js)

- __dummy/__
This folder contains dummy json files for the demo pages

- __fonts/__
This folder contains fonts and their files

- __icons/__
This folder contains icons and their files

- __img/__
This folder contains the dummy images of the theme

- __js/__
Here you will find JS files that do not have bower package wrapper

- __lang/__
This folder contains language specific json files

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

__bower_components/__ This folder contains the bower package files

__documentation/__ Here you will find the documentation of the template (You are reading now this)

__frontend_onepage/__ Here you will find the files of the frontend(onapage) template

__less/__ This folder contains the LESS files for the core styles and bootstrap styles.

  - __app/__ 
    contains the LESS source with the app components
  - __app/themes/__ 
    contains the theme files and variables
  - __app/helpers/__ 
    contains the css helpers of the template
  - __bootstrap/__
    contains the LESS source files for Bootstrap
  - __main.less__
    less include file for the app (app + bootstrap less files)
  - __frontend_onepage.less__
    less include file for the frontend page (app + bootstrap less files)

__node_modules/__ This folder contains the node (npm) modules

__Gruntfile.js__ - contains the grunt environment markup & tasks 

__bower.json__ - contains the bower packages list

__package.json__ - contains the list of the running environment necessary files,compilers (bower,grunt,less compiler)


### How to run it?
#### __1. First step: (install npm dependencies)__

You will need to have installed Node.js (http://nodejs.org/) on your computer.

If you have installed Node.js, you'll need to run a command in the project's root folder:
(Please note that any commands must be ran from the project's root folder.)

``` js
npm install
```

If you issue the above command the dependencies will be installed in the root directory of your project __/node_modules/__. (grunt,bower,grunt tasks...) 

#### __2. Second step: (install javascript dependencies)__

``` js
bower install
```

If you issue the above command the dependencies will be installed in the root directory of your project __/bower_components/__. (Angular/Jquery/3rd party modules/libs/frameworks) 

#### __3. Third step: (run)__

``` js
grunt serve
```

This command executes the Grunt's tasks and starts the web server where the application (will) run(s).
So this will start a local webserver and open up your default browser.

__Note: ha mas webszervert akarsz hasznalni (peldaul apache), akkor az npm es bower install utan csak masold be az egesz konyvtarat a webszerver kiszolgalo konyvtaraba__



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

Watches files for changes and runs tasks based on the changed files, after that your browser will be refreshed automatically.

``` js
grunt clean
```

This command eraises the cache files.

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

This command minifies the concatenated js files of the app which was generated by the previous task (grunt less)


### Less
Less is a CSS pre-processor, meaning that it extends the CSS language, 
adding features that allow variables, mixins, functions and many other 
techniques that allow you to make CSS that is more maintainable, themable 
and extendable.

Less runs inside Node, in the browser and inside Rhino. There are also many 3rd 
party tools that allow you to compile your files and watch for changes.

__You can find YeApp's less files in the less directory__

- LESS files can be found easily because they are separeted per component basis.
For example a table specific less file can be found under the less/app/tables.less path

- The less files of bootstrap are copied into under /less path to avoid the conflict of different versions.

- The bootstrap specific less files are overriden by the application what you can find under /theme directory.

- The less/main.less file stands for the includes of mandatory dependencies.

- The less/fronrtend_onepage.less stands for the includes of mandatory dependencies of the Frontend.

- Note: If you would like to create custom components, we strongly advise that to put the new content into a different file, otherwise it will be overriden.

 - a less fajlok komponensenkent szeparalva vannak kulon fajlokba, azert hogy nagyon
konnyen megtalalhasd amit epp keresel. Pl. ha modositani vagy hozzaadni akarsz a table element
css tulajdonsagaihoz, akkor azt itt keresd: less/app/tables.less

 - a bootstrap less fajljai azert vannak kulon idemasolva (less/bootstrap), hogy ne okozzanak verzio problemakat
 - torekedtunk ra, hogy a bootstrap less fajljait ne modositsuk, ezert a bootstrap element-ek felul vannak irva a /theme konyvtarban

 - less/main.less az angular apphoz szukseges less fajlok gyujtohelye
 - less/frontend_onepage.less a frontendhez szukseges less fajlok gyujtohelye

Note: ha egyedi komponenseket akarsz kesziteni, azokat kulon fajlba tedd, mert yeapp frissites eseten ne keruljenek felulirasra





Main angular modules
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

__ _CONTROLLERS__ - YeApp's controllers and modules

documentation: https://github.com/ocombe/ocLazyLoad 

### UI Router
The de-facto solution to flexible routing with nested views

YeApp's routes are placed in the __app/scripts/app_routes.js__ file.

__Example route config:__

``` js
    .state('components.sortable', {
        url: "/sortable",
        templateUrl: "views/ui-components/sortable.html",
        resolve: resolveRoute(['ng-nestable','ui.sortable'],['jquery.nestable','jquery-ui'])
    })
```

 - Az adott route-hoz termeszetesen betolthetsz futasi idoben fajlokat, oclazyload lib segitsegevel. Ezeket a resolve property megadasaval teheted meg.
resolveRoute fuggveny segit neked eloallitani a resolve objektumot, oly modon, hogy csak a betoltendo script/module nevet adod at neki. (termeszetesen ez csak egy egyszerusites, nyugodtan hasznalhatod az oclazyload defafult resolve
mechnanizmusat). 
    - Elso parametere (array): betolteni kivant angularJS/controllers/modules a _MODULES vagy _CONTROLLERS tombbol (name property)
    - Second parameter (array): betolteni kivant Jquery/3rd party libs a _REQUIRES tombbol (key)

documentation: https://github.com/angular-ui/ui-router

### UI Router breadcrumb

YeApp ui-router is extended with ui-breadrcumb.

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
 - angular ui.router documentation: http://angular-ui.github.io/ui-router/site/#/api/ui.router.state.directive:ui-sref

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

- ahogyan az elso sorban latod, a li taghoz hozzaadodik az 'opened' class ha az aktualis $state tartalmazza a ui route-ot
- $state az egy globalis valtozo, ebben tarolodik el az aktualis route informacio
- lenyilo menu szulojenek, vagyis az a tag-hoz keszitettunk egy directivat (collapse-menu), ami vezerli a lenyilo menu viselkedeset 
- a lenyilo lista elso elemenek egy bizonyos "fold-header"-nek kell lennie, ugyanis ez fixeli a kulonbozo layout elrendezesek problemait, tartalma megegyezik a szulojenek tartalmaval 

- as you can see the first line, you can define "ng-class" property here to detect this
is collapsible item
- $state is a global variable that contains the current tree items of the route. So this example shows if the $state include the "ui" word add the 'opened' class to li tag 
- the collapse "a" html tag has a "collapse-menu" directive. It perform the collapse meachnism (open & close).
- the child ul's first li has to be a "fold-header", this tag is a fixed layout helper for the sidebar. (same as the parent collapse item)


### Header

You can find here: ___app/views/main-header.html__

- a fajlban 2 fo div tag-et talalsz
  - "__navbar-header__": this contains the logo and navbar for mobile(xs) view
  - "__navbar-collapse__": this contains the collapsible menu and navbar for desktop/tablet

### Views/Partials

Ebben a konyvtarban talalod meg a view-kat: __app/views/__

Osszes view komponensenkent szetvannak valogatva a kereshetoseg megkonnyitese erdekeben.
Peldaul: a mail apphoz tartozo html view-kat a app/views/mail konyvtarban fogod megtalalni.



AngularJS
================

### Global app scope - Main.js 

Yeapp-nak van egy root controllere ami a content rootjahoz a body-hoz van definialva.
A root controller -t megtalalod ... mappaban.

A kovetkezo pontokban soroljuk fel a hasznos fuggvenyeket amiket tartalmaz az app. Ezeket 
a fuggvenyeket es valtozokat hasznalhatod kozvetlenul a gyerek controllerekben.
A felsoroltakon kivul vannak meg egyeb valtozok es fuggvenyek amiket csak a demo app-hoz 
hasznalunk.

#### function getLayoutType() 
- ez adja vissza az alkalmazason belul, hogy epp melyik view-ban vagyunk (xs,sm,md,lg).
 Ezeket a breakpoint-okat, az index.html body tagjaban a breakpoint-on belul adhatod meg.

#### function getDefaultSettings() 
- ez a fuggveny adja vissza az app default beallitasait. Ami a kovetkezokeppen nez ki:

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


   - __settings__: layout propertyk amik jelenteserol a Layouts/classes menupont alatt tudsz bovebben olvasni.
   - __settings.theme__: az aktualisan hasznalt theme neve
   - __themes__: app-on belul valaszthato scheme-ek

#### function setDesktopLayout()

Ez a fuggveny gondoskodik, a desktop layout beallitasarol. Bovebben a layouts/desktop layout menupont alatt tudsz rola olvasni.

#### function changeLanguage()

E fuggveny segitsegevel tudod futas idoben valtoztatni a translate nyelvet. 

#### variable mobileLayout:bool 

Ezzel a valtozo segitsegevel tudod lekerdezni barhol az appon belul, hogy most mobile nezetben vagyunk-e.
Erteke true or false lehet


### Add new lib/plugin

####__+Add new default plugin__

There is a possibility to define plugins and libraries which will be downloaded at the time of first page initialization
(Example: AngularJS,Jquery,Oclazyload...)

You can easily add files in the following file: 
'Gruntfile.js' fajlban a 'concat/libs/src' reszben kell bejegyezned a betoltendo lib/framework eleresi utvonalat egy tomb elemekent

__Note for CSS and other files __: You have to register/include your own css and other custom asset files in the head of main index.html.

####__+Add new lazyload plugin__

Mint ahogyan azt mar az Oclazyload menupont alatt emlitettuk, lehetoseg van futasi idoben betolteni js/other fajlokat. Ebben a fajlban talalod meg:  __app/scripts/app_constants.js__

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

### Add new controller/view...

 * __Controllers__ : __app/scripts/controllers__ folder

 * __Views__ : __app/views__ folder

Ha uj controllert akarsz letrehozni csak keszits egy fajlt a controllers mappaban a controller nevevel. Es az elozo pontban emlitett _CONTROLLERS tombe rakd be.

Note: Oclazyload-ban minden futasi idoben betoltott angular komponensnek egy module controllerekent kell lennie. Tehat tulajdonkeppen a controllers konyvtarban module-ok vannak.

### Custom directives

Keszitettunk par egyedi direktivat a theme-hez. __app/scripts/directives/directives.js__


#### __collapseMenu__  
ez a sidebar collapse tulajdonsagaert felel

#### __sparkLine__  
sparkline jquery chart-hoz direktiva.

``` html
<spark-line data="sparkline.inline1.data" options="sparkline.inline1.options"></spark-line>
```

Parameters:
 - data
 - options

#### __morris__  
morris chart-hoz direktiva

``` html
<div id="morris4" morris type="'donut'" options="morris.donut" ></div>
```

Parameters:
 - type
 - options

#### __iCheck__  
icheck pluginhoz direktiva

``` html
<label class="icheck"><input type="checkbox" i-check ng-model="test"> Option one </label>
```

#### __resizeBrowser__ 
ez a direktiva a body taghez van bejegyezve, hogy browser(window) resize eseten az appunkon belul is ertesljuk rola
esemeny neve: resizeBrowser

``` html
<html ng-app="yeappApp" resize-browser>
```

#### __resizeElement__
ezt a direktivat egyeb dom elementekhez jegyezheted fel, es resize eseten broadcastolni fogja az esemenyt
esemeny neve: resizeDomElement

#### __focusMe__
ez a direktiva azert felel, hogy ha az ng-model-ben megadott ertek true lesz, akkor a focus arra az elementre kerul (form control-oknal hasznaljuk)

``` html
<input type="text" class="form-control" placeholder="What needs to be done?" ng-model="newTodo.text" focus-me="list.addMode">
```

#### __vectorMap__ 
jquery vectormap direktivaja

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

If you want to use the basic scrolled layout, you do not have do anything.

### Desktop/Fixed Layout

Ha a desktop layout(fixed)-ot akarod hasznalni, akkor az adott routeodhoz tartozo controllerben megkell hivnod a
root controller (MainCtrl) setDesktopLayout() fuggvenyet true ertekkel. Illetve fel kell iratkoznod a scope destroy esemenyere es a fuggvenyt
false ertekkel kell meghivnod, hogy az app visszaallitsa a default layout-ot. 

(A fuggveny csak hozzadja a 'desktop-layout' class-t a body tagnek)

``` js
    $scope.setDesktopLayout(true);

    $scope.$on("$destroy", function handler() {
        $scope.setDesktopLayout(false);
    });
```

Desktop layout variaciokra peldakat talalsz a app/views/starters mappaban.

Note: ez a layout xs resolutionre nem ervenyes.


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

 * __.themeDefs(1)__ -  in a new theme file you must increment the value (az uj ertek mindig egyel nagyobbnak kell lennie mint az osszes theme osszege)

 * __@themeName__ - the name of the new theme (szokoz nem megengedett!)

 * __@themeBgColor__ - background color of the sidebar

 * __@listItemHoverColor__ - background color of the hovered item of the sidebar

 * __@themeBorderRight__ - border right color of the sidebar

 * __@themeBorderBottom__ - border-bottom of the navbar-brand

 * __@themeFontColor__ - deafult font color of the sidebar

 * __@themeFontHoverColor__ - default font hover color of the sidebar

 * __@themeItemActiveBgColor__ - active item background color of the sidebar

 * __@themeItemActiveFontColor__ - active item font color of the sidebar

 * __@listItemBorderTopColor__ - item border top color of the sidebar

 * __@listItemBorderBottomColor__ - item border bottom color of the sidebar

 * __@listItemActiveBorderTopColor__ - active item border top color of the sidebar

 * __@listItemActiveBorderBottomColor__ - active item border bottom color of the sidebar

#### __3. step (bejegyezni az theme fajlt)__

Az uj fajlt a less/main.less fajl-ban be kell includolni

#### __4. step (megnovelni a loop indexet)__

Megkell novelned a __less/app/theme-generator.less__ fajlban a __@numberOfThemes__ erteket eggyel


 * __Note__: ha barmilyen egyedi css-t akarsz berakni egy theme-be, csak jegyezd be egy less valtozokent, azonban figyelj arra, hogy ezt a variable-t a tobbi theme-ben is bekell jegyezned.
Ezek utan mar csak bekell irnod a 'theme-genarator.less' fajlba, a buldThemes() fuggvenyen belul, hogy ezek az uj css tulajdonsagok hol helyezkedjenek el a DOM tree-ben.



HELPERS
================

### Css helpers

__Note:__

 - ha az other options oszlopban szamokat latsz, az azt jeleneti hogy a class neveben a szamokat ezekre tetszolegesen kicserelheted (mertekegyseg: pixel (px))
 - ha vesszovel felsorolva latsz class-okat azt jelenti hogy mind2re igaz az adott css szabaly

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
|m-3-i | margin:3px !important | 5-10-15-20-30-50 |
|m-t-3 | margin-top:3px !important | 5-10-15-20-30-50 |
|m-b-3 | margin-bottom:3px !important | 5-10-15-20-30-50 |
|m-r-3 | margin-right:3px !important | 5-10-15-20-30-50 |
|m-l-3 | margin-left:3px !important | 5-10-15-20-30-50 |
|m-t-b-3,p-b-t-3 | margin-top:3px !important & margin-bottom:3px !important | 5-10-15-20-30-50 |
|m-r-l-3,p-l-r-3 | margin-right:3px !important & margin-left:3px !important | 5-10-15-20-30-50 |

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

- These classes helps you to separate your panels or boxes.

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

- If you want an absolute position element in your DOM, just add the "item" class to your parent element. Az abszolut pozicionalasu element-nek csak add meg a wrapper classt, illetve az elhelyezkedeset (top,bottom,left,right)

#### Table layout

| Name | Description          | Comment          |
| ------------- | ----------- | ----------- | |
| r-sm-table     | display:table  |  |
| col-sm-cell,c-sm-cell |  display:table-cell   | &nbsp;  |
| v-middle |  vertical-align: middle   | &nbsp;  |
| v-top |  vertical-align: top   | &nbsp;  |
| v-bottom |  vertical-align: bottom   | &nbsp;  |

Ezek a classok mobil nezet kivetelevel az osszes resolutionben mukodnek

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
We offer free support and updates to our valuable customers!

SUPPORT
================
You can request for support via themeforest comments.

We will assist you any problem you face while buidling your app via YeApp framework.
