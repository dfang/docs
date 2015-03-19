# build your workflow with gulp

### Optimize or Compile
[gulp-uglify](https://www.npmjs.com/package/gulp-uglify) Minify files with UglifyJS  
[gulp-concat](https://www.npmjs.com/package/gulp-concat) Concatenates files  
[gulp-minify-html](https://www.npmjs.com/package/gulp-minify-html) Minify html with minimize  
[gulp-minify-css](https://www.npmjs.com/package/gulp-minify-css) Minify css with clean-css or gulp-csso  
[gulp-sourcemaps](https://www.npmjs.com/package/gulp-sourcemaps) Source map support for Gulp.js  
[gulp-less](https://www.npmjs.com/package/gulp-less)  Compile less  
[gulp-sass](https://www.npmjs.com/package/gulp-sass)  Compile sass  
[gulp-typescript](https://www.npmjs.com/package/gulp-typescript)  Compile typescript  
[gulp-coffee](https://www.npmjs.com/package/gulp-coffee)  Compile coffeescript  
[gulp-rev](https://www.npmjs.com/package/gulp-rev)  Static asset revisioning  


### Code Sytle or Lint or Hint
[gulp-jscs](https://github.com/jscs-dev/gulp-jscs) Check JavaScript code style with jscs  
[gulp-jshint](https://www.npmjs.com/package/gulp-jshint) JSHint plugin for gulp  

### Plugins for angular js
[gulp-ngtemplate](https://www.npmjs.com/package/gulp-ngtemplate) or [gulp-ng-html2js](https://www.npmjs.com/package/gulp-ng-html2js) or [gulp-angular-templatecache
](https://www.npmjs.com/package/gulp-angular-templatecache) Gulp task to precompile AngularJS templates with $templateCache  
[gulp-ng-annotate](https://www.npmjs.com/package/gulp-ng-annotate) Add angularjs dependency injection annotations with ng-annotate  
[gulp-ng-classify](https://www.npmjs.com/package/gulp-ng-classify) Compile CoffeeScript classes to AngularJS modules  


### Customize Workflow
[browser-sync](http://browsersync.io) livreload server and cross device testing  
[gulp-list](https://www.npmjs.com/package/gulp-list) Gulp task lister  
[gulp-notify](https://www.npmjs.com/package/gulp-notify) notification plugin for gulp  
[gulp-plumber](https://github.com/floatdrop/gulp-plumber) Fix for Node pipes panic unpiping on error(By design, Node stream will stop accepting incoming data, if error event was raised)
[gulp-flatten](https://www.npmjs.com/package/gulp-flatten) remove or replace relative path for files  
[gulp-filter](https://www.npmjs.com/package/gulp-filter) Filter files in a vinyl stream  
[gulp-if](https://www.npmjs.com/package/gulp-if) Conditionally run a task  
[gulp-ignore](https://github.com/robrich/gulp-ignore) plugin for gulp to ignore files in the stream based on file characteristics  
[gulp-rename](https://www.npmjs.com/package/gulp-rename) Rename files easily  
[gulp-replace](https://www.npmjs.com/package/gulp-replace) A string replace plugin for gulp  
[del](https://www.npmjs.com/package/del)  A gulp plugin for removing files and folders  or [gulp-clean](https://www.npmjs.com/package/gulp-clean)  
[merge2](https://www.npmjs.com/package/merge2) Merge multiple streams into one stream in sequence or parallel  
[gulp-order](https://www.npmjs.com/package/gulp-order) allows you to reorder a stream of files using the same syntax as of gulp.src  

[gulp-ngdocs](https://www.npmjs.com/package/gulp-ngdocs) gulp plugin for angularjs-like documentation  
[gulp-header](https://www.npmjs.com/package/gulp-header) add header to file(s) in the pipeline  

### Load gulp tasks
[requireDir](https://github.com/aseemk/requireDir)  
[gulp-task-loader](https://www.npmjs.com/package/gulp-task-loader)  
[gulp-loader](https://www.npmjs.com/package/gulp-loader)  
[gulp-load-plugins](https://www.npmjs.com/packages/gulp-load-plugins)  


### Inject build bock
[wiredep](https://github.com/taptapship/wiredep)  Wire dependencies to your source code  
[gulp-bower-files](https://www.npmjs.com/package/gulp-bower-files) Build gulp.src() of your bower packages main files  
[bower-main](https://www.npmjs.com/package/bower-main) Get bower main files in both normal and in minimized formats, bower.
gulp-bower-main: uses bower-main-files and manipulates the result, now is deprecated. bower-main use bower-main-files too  
[gulp-bower-overrides](https://www.npmjs.com/package/gulp-bower-overrides)  merge bower overrides into bower.json files  

[gulp-useref](https://www.npmjs.com/package/gulp-useref) Parse build blocks in HTML files to replace references to non-optimized scripts or stylesheets  
[gulp-inject](https://www.npmjs.com/package/gulp-inject) A javascript, stylesheet and webcomponent injection plugin for Gulp, i.e. inject file references into your index.html  
[gulp-html-replace](https://www.npmjs.com/package/gulp-html-replace) Replace build blocks in HTML. Like useref but done right  
[gulp-usemin](https://www.npmjs.com/package/gulp-usemin)  Replaces references to non-optimized scripts or stylesheets into a set of HTML files (or any templates/views)  


### Recipes
https://github.com/gulpjs/gulp/tree/master/docs/recipes  
https://github.com/google/web-starter-kit/blob/master/gulpfile.js  
https://github.com/osscafe/gulp-cheatsheet  
http://www.smashingmagazine.com/2014/06/11/building-with-gulp/  
[generator-gulp-angular](https://github.com/Swiip/generator-gulp-angular)


### Notes

关于server or livereload, 不需要http-server, gulp-livereload, gulp-nodemon等, 一个[browserSync](www.browsersync.io)全搞定(自带watch, open browser, livereload 等功能)  

关于loading gulp tasks 可以创建一个gulp文件夹, 把task分割成文件, 用require-dir 或 gulp-task-loader  or gulp-loader 加载

有些功能能做到的插件有很多(比如自动插入引用到index.html或 ng template cache), 还需要进一步比较  

如果不知道怎么写task, 可以参考recipes里的链接, 也可以从gulp-angular-generator生成的gulpfile.js借用  
