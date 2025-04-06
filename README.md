# Rick Sanchez Ipsum Generator

[![StyleCI](https://github.styleci.io/repos/961243233/shield?branch=master)](https://github.styleci.io/repos/961243233?branch=master)
[![Composer Install](https://github.com/jeremykenedy/rick-sanchez-ipsum/actions/workflows/php.yml/badge.svg)](https://github.com/jeremykenedy/rick-sanchez-ipsum/actions/workflows/php.yml)
[![App Version](https://img.shields.io/github/v/tag/jeremykenedy/rick-sanchez-ipsum.svg?sort=semver&label=App%20Version)](https://github.com/jeremykenedy/rick-sanchez-ipsum/releases)
[![License: MIT](https://img.shields.io/static/v1?label=License&message=MIT&color=green&style=flat)](https://opensource.org/licenses/MIT)

### Table of contents
- [About](#about)
- [Features](#features)
- [Installation Instructions](#installation-instructions)
    - [Build the Front End Assets with Vite](#build-the-front-end-assets-with-vitejs)
    - [Optionally Build Cache](#optionally-build-cache)
- [Screenshots](#screenshots)
- [File Tree](#file-tree)
- [License](#license)

## About
A Laravel + Vite + Vue 3 + TailwindCSS Rick Sanchez Ipsum Generator.
Uses official [TailwindCSS](https://tailwindcss.com/). While the front end is
part of this repository it is a completely separated Vue 3 front end compiled using ViteJS.

## App Features
##### Built on:
- [✅ Laravel 12](https://github.com/laravel/laravel)
- [✅ Vite](https://laravel.com/docs/9.x/vite)
- [✅ Vue 3](https://github.com/vuejs/vue)
- [✅ TailwindCSS (w/ `@tailwindcss/forms` and `@tailwindcss/aspect-ratio`)](https://tailwindcss.com/)
- [✅ VueRouter](https://router.vuejs.org/)
- [✅ Pinia](https://pinia.vuejs.org/)
- [✅ Headless UI](https://headlessui.com/)
- [✅ Heroicons](https://heroicons.com/)
- [✅ ESLint](https://eslint.org/) with [✅ Prettier](https://prettier.io/docs/en/index.html)

##### Features:
- Home Page
- 404 Page
- [Google Analytics (optional)](https://matteo-gabriele.gitbook.io/vue-gtag/v/next/)

## Installation Instructions
1. Run `git clone https://github.com/jeremykenedy/rick-sanchez-ipsum.git rick-sanchez-ipsum`
2. From the projects root run `cp .env.example .env`
3. Configure your `.env` file
4. Run `composer install` from the projects root folder
5. From the projects root folder run `sudo chmod -R 755 ../rick-sanchez-ipsum`
6. From the projects root folder run `php artisan key:generate`
7. Compile the front end assets with [npm steps](#using-npm) or [yarn steps](#using-yarn).

#### Build the Front End Assets with ViteJs
##### Using NPM:
1. From the projects root folder run `npm install`
2. From the projects root folder run `npm run dev` or `npm run build`
  * You can lint assets with `npm run lint`
  * You can clean the syntax with `npm run clean`

##### Using Yarn:
1. From the projects root folder run `yarn install`
2. From the projects root folder run `yarn run dev` or `yarn run build`
  * You can lint assets with `yarn run lint`
  * You can clean the syntax with `yarn run clean`

###### And thats it with the caveat of setting up and configuring your development environment.

## Screenshots

<p float="left">
    <img src="https://rick-sanchez-ipsum.s3.us-west-2.amazonaws.com/home-light.png" title="Home Page Light Mode" alt="Home Page Light Mode" width="48%"/>
    <img src="https://rick-sanchez-ipsum.s3.us-west-2.amazonaws.com/home-dark.png" title="Home Page Dark Mode" alt="Home Page Dark Mode" width="48%"/>
    <img src="https://rick-sanchez-ipsum.s3.us-west-2.amazonaws.com/404-light.png" title="404 Page Light Mode" alt="404 Page Light Mode" width="48%"/>
    <img src="https://rick-sanchez-ipsum.s3.us-west-2.amazonaws.com/404-dark.png" title="404 Page Dark Mode" alt="404 Page Dark Mode" width="48%"/>
</p>

## File Tree
```
.
├── .editorconfig
├── .env.example
├── .eslintrc.js
├── .eslintrc.json
├── .gitattributes
├── .github
│   ├── FUNDING.yml
│   ├── dependabot.yml
│   ├── labeler.yml
│   └── workflows
│       ├── build-changelog.yml
│       ├── dependency-review.yml
│       ├── deploy.yml
│       ├── greetings.yml
│       ├── labeler.yml
│       ├── laravel.yml
│       ├── node.js.yml
│       ├── php.yml
│       └── stale.yml
├── .gitignore
├── .prettierignore
├── .prettierrc.json
├── .scripts
│   └── deploy.sh
├── .styleci.yml
├── LICENSE
├── README.md
├── SECURITY.md
├── app
│   ├── Console
│   │   └── Kernel.php
│   ├── Exceptions
│   │   └── Handler.php
│   ├── Http
│   │   ├── Kernel.php
│   │   └── Middleware
│   │       ├── EncryptCookies.php
│   │       ├── PreventRequestsDuringMaintenance.php
│   │       ├── TrimStrings.php
│   │       ├── TrustHosts.php
│   │       ├── TrustProxies.php
│   │       └── VerifyCsrfToken.php
│   └── Providers
│       ├── AppServiceProvider.php
│       └── RouteServiceProvider.php
├── artisan
├── bootstrap
│   ├── app.php
│   └── cache
│       ├── .gitignore
│       ├── packages.php
│       └── services.php
├── composer.json
├── composer.lock
├── config
│   ├── app.php
│   ├── logging.php
│   ├── services.php
│   └── settings.php
├── eslint.config.js
├── package-lock.json
├── package.json
├── postcss.config.js
├── prettier.config.js
├── public
│   ├── .htaccess
│   ├── android-chrome-192x192.png
│   ├── android-chrome-512x512.png
│   ├── apple-touch-icon.png
│   ├── favicon-16x16.png
│   ├── favicon-32x32.png
│   ├── favicon.ico
│   ├── favicon.png
│   ├── index.php
│   ├── robots.txt
│   ├── serviceworker.js
│   ├── site.webmanifest
│   └── sw.js
├── resources
│   ├── css
│   │   ├── app.css
│   │   └── normalize.css
│   ├── img
│   │   ├── 404-light.png
│   │   ├── 404.png
│   │   ├── favicon
│   │   │   ├── android-chrome-192x192.png
│   │   │   ├── android-chrome-512x512.png
│   │   │   ├── apple-touch-icon.png
│   │   │   ├── favicon-16x16.png
│   │   │   ├── favicon-32x32.png
│   │   │   ├── favicon.ico
│   │   │   ├── favicon.png
│   │   │   └── site.webmanifest
│   │   └── logo
│   │       ├── logo-dark.png
│   │       ├── logo-light.png
│   │       ├── main-dark.png
│   │       └── main-light.png
│   ├── js
│   │   ├── app.js
│   │   ├── bootstrap.js
│   │   ├── components
│   │   │   ├── ToggleDarkMode.vue
│   │   │   ├── common
│   │   │   │   └── AppButton.vue
│   │   │   ├── includes
│   │   │   │   ├── AppFooter.vue
│   │   │   │   └── AppNav.vue
│   │   │   └── ipsums
│   │   │       └── IpsumComponent.vue
│   │   ├── composables
│   │   │   └── darkmode.js
│   │   ├── layouts
│   │   │   └── GuestLayout.vue
│   │   ├── routes
│   │   │   ├── index.js
│   │   │   └── routes.js
│   │   ├── services
│   │   │   ├── analytics.js
│   │   │   └── words.js
│   │   ├── store
│   │   │   ├── index.js
│   │   │   └── toast.js
│   │   └── views
│   │       ├── errors
│   │       │   └── NotFound.vue
│   │       └── home
│   │           └── HomePage.vue
│   └── views
│       └── app.blade.php
├── routes
│   └── web.php
├── tailwind.config.js
├── tailwindcss-perspective.js
├── vite.config.js
└── vue.config.js

34 directories, 104 files

```

* Tree command can be installed using brew: `brew install tree`
* File tree generated using command `tree -a -I '.git|node_modules|vendor|build|storage|tests|.DS_Store|.env'`

## License
Rick Sanchez Ipsum Generator is licensed under the [MIT license](https://opensource.org/licenses/MIT). Enjoy!
