<p align="center">
  <a href="https://laravel.com">
    <img src="https://img.shields.io/badge/laravel-7.3-brightgreen.svg" alt="vue">
  </a>
  <a href="https://github.com/vuejs/vue">
    <img src="https://img.shields.io/badge/vue-2.6.10-brightgreen.svg" alt="vue">
  </a>
  <a href="https://github.com/ElemeFE/element">
    <img src="https://img.shields.io/badge/element--ui-2.13.0-brightgreen.svg" alt="element-ui">
  </a>
  <a href="https://github.com/tuandm/laravue/blob/master/LICENSE">
    <img src="https://img.shields.io/badge/license-MIT-brightgreen.svg" alt="license">
  </a>
</p>

# 
 This Application is a beautiful dashboard combination of [Laravel](https://laravel.com/), [Vue.js](https://github.com/vuejs/vue) and the UI Toolkit [Element](https://github.com/ElemeFE/element). The work is inspired by  [vue-element-admin](http://panjiachen.github.io/vue-element-admin) with our love on top of that. With the powerful Laravel framework as the backend, Vue.js as the high performance on the frontend,  Laravue appears to be a full-stack solution for an enterprise application level.

## Screenshot
<p align="center">
  <img width="900" src="https://cdn.laravue.dev/screenshot.png">
</p>

## Getting started

### Prerequisites

 * Laravue is positioned as an enterprise management solution, and it is highly recommended to use it to start from scratch.
 * For existing Laravel project, you should check [Laravue Core](https://github.com/tuandm/laravue-core) for integration.
 * Your machine needs to be ready for the latest [Laravel](https://laravel.com/docs/6.x#installation) and [Node.js](https://nodejs.org).


### Installing
#### Manual

```bash
# Clone the project and run composer
composer create-project tuandm/laravue
cd laravue

# Migration and DB seeder (after changing your DB settings in .env)
php artisan migrate --seed

# Install dependency with NPM
npm install

# develop
npm run dev # or npm run watch

# Build on production
npm run production
```

#### Docker
```sh
docker-compose up -d
```
Build static files within Laravel container with npm
```sh
# Get laravel docker container ID from containers list
docker ps

docker exec -it <container ID> npm run dev # or npm run watch
# Where <container ID> is the "laravel" container name, ex: src_laravel_1
```
Open http://localhost:8000 (laravel container port declared in `docker-compose.yml`) to access Laravue

## Running the tests
* Tests system is under development

## Deployment and/or CI/CD
This project uses [Envoy](https://laravel.com/docs/5.8/envoy) for deployment, and [GitLab CI/CD](https://about.gitlab.com/product/continuous-integration/). Please check `Envoy.blade.php` and `.gitlab-ci.yml` for more detail.

## Built with
* [Laravel](https://laravel.com/) - The PHP Framework For Web Artisans
* [Laravel Sanctum](https://github.com/laravel/sanctum/) - Laravel Sanctum provides a featherweight authentication system for SPAs and simple APIs.
* [spatie/laravel-permission](https://github.com/spatie/laravel-permission) - Associate users with permissions and roles.
* [VueJS](https://vuejs.org/) - The Progressive JavaScript Framework
* [Element](https://element.eleme.io/) - A  Vue 2.0 based component library for developers, designers and product managers
* [Vue Admin Template](https://github.com/PanJiaChen/vue-admin-template) - A minimal vue admin template with Element UI


## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, please look at the [release tags](https://github.com/tuandm/laravue/tags) on this repository.

## Acknowledgements

* [vue-element-admin](https://panjiachen.github.io/vue-element-admin/#/) A magical vue admin which insprited Laravue project.
* [tui.editor](https://github.com/nhnent/tui.editor) - Markdown WYSIWYG Editor.
* [Echarts](http://echarts.apache.org/) - A powerful, interactive charting and visualization library for browser.

