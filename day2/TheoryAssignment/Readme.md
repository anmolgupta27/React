What is `NPM`?
  - NPM is two things, first and foremost it is an online repository for publishing open source node projects and second, it is a command line utility for interacting with said repository that aid package installation, version management and dependency management
  ex: -> npm install -D parcel - this will install parcel in my node modules and we are all set to use this beast

What is `Parcel/Webpack`? Why do we need it?
 - Parcel is a beast.
 - It is a bundler which will create help us to create a production ready app.
 - It comes up some extra tools to perform, HMR(hot module replacement), caching, image optimization, compression, lazy loading, clean up our code, minify, compatible with old version of browsers

What is `.parcel-cache`
 - In cache folder parcel stores the information about our project when it builds so that when it rebuild it doesnot have to start analyze everything from scratch, that is one of the reason why parcel is fast in development mode, it just compare what changes and build that

What is `npx` ?
 - NPX stand for node package execute it comes with npm and it will execute the package you want to run
 For ex. -> npx parcel index.html -> it will start executing the parcel to create a development build and run a live server

What is difference between `dependencies` vs `devDependencies`
 - dependencies are one which is required on production and that is installed transitively means if a requires b and b requires c then C get installed otherwise neither B could work nor A.
 - devDependencies are one which is required only for development purpose like babel, jest and some testing things.

What is Tree Shaking?
 - Tree shaking is a technique to remove dead code from the build.
 - It relies on import and export statement of a component that will help in order to understand the usage of that component in different javascript files.
 - Bundlers mostly using this technique to remove unwanted code from the build and create a production ready build with minified and small size files

What is Hot Module Replacement?
 - Hot reloading is one that parcel will do in the development phase when you make any changes then parcel will rebuild it and update the page / reload the page with the updated build and your changes will reflect on webpage
 but in some of the cases complete page reload is not required so in that case HMR (hot module replacement) comes
 in picture where it will just replace that module with the updated one at runtime, like when you are updating any css

List down your favourite 5 superpowers of Parcel and describe any 3 of them in your
own words.
 - Shared bundles
 - Caching
 - Compression
 - Image Optimization
 - lazy mode

 - Image optimization -> Parcel providing out of box support to resizing, converting, and optimizing images, supported format are jpg, png, webp, avif
 query parameters are - width, height, quality, as
 src="image.jpeg?as=webp&widht=250px",
 It will optimize lossless jpg, png on production without impacting quality, we can disable this on production

 -Lazy mode- it becomes frustating for the developer to wait for all the pages to build on development mode, so with the help of --lazy mode we can tell parcel to build the pages when user visit on those pages and when user visit parcel build only those files that is required to serve that page. this will help in order to reduce the development build time and development becomes faster

 - Shared bundles - any part of code or module which is being used in two different pages or places then parcel will share that bundle in both the bundles so that dependencies can be loaded in parallel and cached separately

What is `.gitignore`? What should we add and not add into it?
 - it is file being used to track all the thing which is not required to push to the project repository.
 - We should add those things that can be regenerated like node_modules, dist, .parcel_cache

What is the difference between `package.json` and `package-lock.json`
 - package.json is a versioning file being used to install multiple package manager in your project and package-lock.json will the lock the installed version of the package and will install that locked version

Why should I not modify `package-lock.json`?
 - we should never modify the package-lock as it is having the exact locked version that is being used in our project.

What is `node_modules` ? Is it a good idea to push that on git?
 - node_modules is like a cache for external modules that your project is depend upon. when you install any package it will get installed in node_modules and after that we are all set to use that package by importing in our application. It should never be pushed to git as it is very heavy file.

What is the `dist` folder?
 - dist folder is having production ready build of our application

What is `browserlists
 - Browserlists is a tool with the help of that we are specifying that which version or browser we want to get support for our applicaton.
















