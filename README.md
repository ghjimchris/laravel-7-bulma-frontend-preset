# Bulma Frontend Preset For Laravel 7 and Up

Bulma Frontend Preset For Laravel Framework 7 and Up

*Current version*: **Bulma ^v0.8.0** + **Bulma Extensions ^v6.2.7**

## Install
Install this preset via `composer require laravel-7-frontend-presets/bulma`.

and follow instructions below.

## Usage
1. Fresh install Laravel 7 (and up) and `cd` to your app.
2. Install this preset via `composer require laravel-7-frontend-presets/bulma`. No need to register the service provider. Laravel 5.5 & up can auto detect the package.
3. Use `php artisan ui bulma` for basic Bulma preset. **OR** Use `php artisan ui bulma --auth` for basic preset, Auth route entry and Bulma Auth views in one go.
4. `npm install`
5. `npm run dev`
6. `npm run dev` will give you an error: vertical-align: middle;
7. go to node_modules then bulma-extension then bulma-slider then sass and edit the index.sass at line 86 delete the ; you only need vertical-align: middle and same with line 91 delete the ;
8. `npm run dev` it should works now.
9. Configure your favorite database (mysql, sqlite etc.)
10. `php artisan migrate` to create basic user tables.
11. `php artisan serve` (or equivalent) to run server and test preset.

## Bulma Pagination Template
1. Upto Laravel 5.6 - Vendor publish and replace the code from here [default.blade.php](https://gist.github.com/Laraveldeep/0797c5a4079e3a2a0ba5b2b0e98f0357)
1. Laravel 5.7 and up - Vendor publish and replace the code from here [bootstrap-4.blade.php](https://gist.github.com/Laraveldeep/362490aead2fc4b2fd15c3aae24254cf)

## Bulma Extensions
1. It is a set of missing [Bulma.io](https://bulma.io/) functionalities in the form of extensions. More info at [https://wikiki.github.io/](https://wikiki.github.io/)
2. Customize `bulma.sass`, `bulma-extensions.sass`, `bulma-extensions.js` and `app.js` as needed.

## Screenshots
![Bulma login screen](/screenshots/Laravel_7_bulma_frontend.jpg)
![Bulma login screen](/screenshots/bulma_login_screen.jpg)
