A simple template for Drupal 7.

## Technologies:

* Based on [`drupal-project`](github.com/drupal-composer/drupal-project)
* [Docker](https://www.docker.com/) and Docker Compose

## Usage:

Run `composer install` and `docker-compose up -d`.

Custom modules are a bit tricky. Using [custom install paths](https://github.com/composer/installers#custom-install-paths), you can specify where you're custom module will be installed. An option is to add a single directory as a composer package and make it a dependency. You can then include all custom modules inside that directory. An example is `modules/dsdeiz-default` which has a package named `dsdeiz/default`. All modules can be included inside that directory. You can separate your modules as well but you will need to define a `composer.json` for each package/module.
