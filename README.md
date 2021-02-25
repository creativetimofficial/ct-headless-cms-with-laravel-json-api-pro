# [Headless CMS with Laravel JSON:API PRO](https://headless-cms-with-laravel-json-api.creative-tim.com/?ref=hclja-readme)

![version](https://img.shields.io/badge/version-1.0.0-blue.svg) [![GitHub issues open](https://img.shields.io/github/issues/creativetimofficial/ct-headless-cms-with-laravel-json-api.svg?maxAge=2592000)](https://github.com/creativetimofficial/ct-headless-cms-with-laravel-json-api/issues?q=is%3Aopen+is%3Aissue) [![GitHub issues closed](https://img.shields.io/github/issues-closed-raw/creativetimofficial/ct-headless-cms-with-laravel-json-api/ct-headless-cms-with-laravel-json-api.svg?maxAge=2592000)](https://github.com/creativetimofficial/ct-headless-cms-with-laravel-json-api/issues?q=is%3Aissue+is%3Aclosed)

![Product Image](https://github.com/creativetimofficial/public-assets/raw/master/headless-cms-with-laravel-json-api/headless-cms-with-laravel-json-api.jpg?raw=true)

Laravel Headless CMS follows the JSON:API standard for building APIs in JSON. JSON:API is a specification for how a client should request that resources be fetched or modified, and how a server should respond to those requests. It`s specifically designed to increase efficiency by keeping the number of requests and the amount of data transmitted between clients and servers to a minimum.  

# Download
Download the .zip file from the Creative Tim site and extract it.

# Laravel API Setup

## Introduction

JSON:API is a specification for how a client should request that resources be fetched or modified, and how a server should respond to those requests. It is designed to minimize both the number of requests and the amount of data transmitted between clients and servers. This efficiency is achieved without compromising readability, flexibility, or discoverability.

[Click here to go to the JSON:API docs](https://explore.postman.com/api/6357/laravel-jsonapi)

## Prerequisites

The Laravel JSON:API backend project requires a proper multi-threaded web server such as Apache/Nginx environment with PHP, Composer and MySQL.

**Do not use `php artisan serve` as it will result in stalled requests due to the single-threaded nature of the built-in PHP web server.** 

We strongly recommend using [Laradock](https://laradock.io/) for Linux and Mac or [Laragon](https://laragon.org/download/) for Windows if possible.

Other options for your local environment:
- Windows: [How to install WAMP on Windows](https://updivision.com/blog/post/beginner-s-guide-to-setting-up-your-local-development-environment-on-windows)
- Linux: [How to install LAMP on Linux](https://howtoubuntu.org/how-to-install-lamp-on-ubuntu)
- Mac: [How to install MAMP on MAC](https://wpshout.com/quick-guides/how-to-install-mamp-on-your-mac/)

You will also need to install Composer 2: [https://getcomposer.org/doc/00-intro.md](https://getcomposer.org/doc/00-intro.md)

## Laravel JSON:API Project Installation

1. Navigate in your Laravel API project folder: `cd your-laravel-json-api-project`
2. Install project dependencies: `composer install`
3. Create a new .env file: `cp .env.example .env`
3. Add your own database credentials in the .env file in DB_DATABASE, DB_USERNAME, DB_PASSWORD
5. Create users table: `php artisan migrate --seed`
6. Generate application key: `php artisan key:generate`
7. Install Laravel Passport: `php artisan passport:install`
8. Add your own mailtrap.io credentials in MAIL_USERNAME and MAIL_PASSWORD in the .env file

## Usage

You can register as a user or log in using one of the default users: 

- admin type - **admin@jsonapi.com** with the password **secret**
- creator type - **creator@jsonapi.com** with the password **secret**
- member type - **member@jsonapi.com** with the password **secret**

A **member type** user can log in, update his profile and view a list of added items.  
A **creator type** user can log in, update his profile and perform actions on categories, tags and items.
A **admin type** user can log in, update his profile and perform actions on categories, tags, items, roles and users.

Headless CMS with Laravel JSON:API PRO provides basic CRUD endpoints for the most commonly used functionalities in any CMS. 

* Authentication API: login, logout, register, send reset password email & reset password
* Profile API: get profile, update profile
* Users API: list, create, update and delete users, upload profile image
* Roles API: list, create, edit and remove roles
* Permissions API: list available permissions
* Tags API: list, create, update and delete tags
* Categories API: list, create, update and delete categories
* Items API: list, create, update, delete items & upload item image

## Table of Contents

* [Versions](#versions)
* [Documentation](#documentation)
* [Dashboards built with Headless CMS with Laravel JSON:API PRO](#dashboards-built-with-headless-cms-with-laravel-json-api-pro)
* [Resources](#resources)
* [Reporting Issues](#reporting-issues)
* [Licensing](#licensing)
* [Useful Links](#useful-links)

## Versions

[<img src="https://github.com/creativetimofficial/public-assets/blob/master/logos/laravel_logo.png" height="80" />](#)
[<img src="https://github.com/creativetimofficial/public-assets/blob/master/logos/json-api.png" height="75" />](#)

## Documentation
The documentation for the Headless CMS with Laravel JSON:API PRO is hosted at our [here](https://explore.postman.com/api/6357/laravel-jsonapi).

## Resources
- Download Page: <https://www.creative-tim.com/product/headless-cms-with-laravel-json-api-pro>
- Documentation: <https://explore.postman.com/api/6357/laravel-jsonapi>
- License Agreement: <https://www.creative-tim.com/license>
- Support: <https://www.creative-tim.com/contact-us>
- Issues: [Github Issues Page](https://github.com/creativetimofficial/ct-headless-cms-with-laravel-json-api-pro/issues)

## Dashboards built with Headless CMS with Laravel JSON:API PRO
| Vue Argon Dashboard Laravel | Vue Material Dashboard Laravel |
| --- | --- |
| [![Vue Argon Dashboard Pro Laravel](https://s3.amazonaws.com/creativetim_bucket/products/353/original/opt_adp_vue_laravel_thumbnail.jpg)](https://www.creative-tim.com/product/vue-argon-dashboard-pro-laravel?ref=hclja-readme) | [![Vue Material Dashboard Laravel Pro](https://s3.amazonaws.com/creativetim_bucket/products/332/original/opt_mdp_vuelaravel_thumbnail.jpg)](https://www.creative-tim.com/product/vue-material-dashboard-laravel-pro?ref=hclja-readme) |

| Vue Black Dashboard Laravel | Vue White Dashboard Laravel |
| --- | --- |
| [![Vue Black Dashboard Pro Laravel](https://s3.amazonaws.com/creativetim_bucket/products/403/original/opt_bdp_vuelaravel_thumbnail.jpg)](https://www.creative-tim.com/product/vue-black-dashboard-pro-laravel?ref=vbdpl-readme) | [![Vue White Dashboard Pro Laravel](https://s3.amazonaws.com/creativetim_bucket/products/409/original/opt_wdp_vuelaravel_thumbnail.jpg)](https://www.creative-tim.com/product/vue-white-dashboard-pro-laravel?ref=vwdpl-readme) |

| Vue Paper Dashboard Laravel | Vue Now UI Dashboard Laravel |
| --- | --- |
| [![Vue Paper Dashboard Pro Laravel ](https://s3.amazonaws.com/creativetim_bucket/products/405/original/opt_pdp_vuelaravel_thumbnail.jpg)](https://www.creative-tim.com/product/vue-paper-dashboard-pro-laravel?ref=vpdpl-readme) | [![Vue Now UI Dashboard Pro Laravel ](https://s3.amazonaws.com/creativetim_bucket/products/407/original/opt_nudp_vuelaravel_thumbnail.jpg)](https://www.creative-tim.com/product/vue-now-ui-dashboard-pro-laravel?ref=vnudpl-readme) |

| Nuxt Argon Dashboard Laravel |
| --- |
| [![Nuxt Argon Dashboard Pro Laravel](https://s3.amazonaws.com/creativetim_bucket/products/351/original/opt_adp_nuxt_laravel_thumbnail.jpg)](https://www.creative-tim.com/product/nuxt-argon-dashboard-pro-laravel?ref=hclja-readme) |



## Change log

Please see the [changelog](CHANGELOG.md) for more information on what has changed recently.

## Reporting Issues

We use GitHub Issues as the official bug tracker for the Headless CMS with Laravel JSON:API PRO. Here are some advices for our users that want to report an issue:

1. Make sure that you are using the latest version of the Headless CMS with Laravel JSON:API PRO. Check the CHANGELOG from your dashboard on our [website](https://www.creative-tim.com/?ref=hclja-readme).
2. Providing us reproducible steps for the issue will shorten the time it takes for it to be fixed.
3. Some issues may be browser specific, so specifying in what browser you encountered the issue might help.

## Licensing

- Copyright Creative Tim (https://www.creative-tim.com/?ref=hclja-readme)
- Creative Tim License (https://www.creative-tim.com/license).


## Useful Links

- [Tutorials](https://www.youtube.com/channel/UCVyTG4sCw-rOvB9oHkzZD1w)
- [Affiliate Program](https://www.creative-tim.com/affiliates/new) (earn money)
- [Blog Creative Tim](http://blog.creative-tim.com/)
- [Free Products](https://www.creative-tim.com/bootstrap-themes/free) from Creative Tim
- [Premium Products](https://www.creative-tim.com/bootstrap-themes/premium?ref=hclja-readme) from Creative Tim
- [React Products](https://www.creative-tim.com/bootstrap-themes/react-themes?ref=hclja-readme) from Creative Tim
- [Angular Products](https://www.creative-tim.com/bootstrap-themes/angular-themes?ref=hclja-readme) from Creative Tim
- [VueJS Products](https://www.creative-tim.com/bootstrap-themes/vuejs-themes?ref=hclja-readme) from Creative Tim
- [More products](https://www.creative-tim.com/bootstrap-themes?ref=hclja-readme) from Creative Tim
- Check our Bundles [here](https://www.creative-tim.com/bundles??ref=hclja-readme)

## Social Media

### Creative Tim:

Twitter: <https://twitter.com/CreativeTim?ref=hclja-readme>

Facebook: <https://www.facebook.com/CreativeTim?ref=hclja-readme>

Dribbble: <https://dribbble.com/creativetim?ref=hclja-readme>

Instagram: <https://www.instagram.com/CreativeTimOfficial?ref=hclja-readme>


### Updivision:

Twitter: <https://twitter.com/updivision?ref=hclja-readme>

Facebook: <https://www.facebook.com/updivision?ref=hclja-readme>

Linkedin: <https://www.linkedin.com/company/updivision?ref=hclja-readme>

Updivision Blog: <https://updivision.com/blog/?ref=hclja-readme>

## Credits

- [Creative Tim](https://creative-tim.com/?ref=hclja-readme)
- [UPDIVISION](https://updivision.com)
