# d7-cfr-recommended
Meta package to require the most common / recommended cfr-related modules in D7.

## Installation

First install your Drupal 7 website with something like https://github.com/drupal-composer/drupal-project/tree/7.x.

    composer create-project drupal-composer/drupal-project:7.x-dev some-dir --no-interaction

Create a database and install Drupal 7.

Then require this package:

    cd some-dir
    composer require donquixote/d7-cfr-recommended

Then enable modules with drush.

    cd web
    drush en -y entdisp listformat entdisp_example cfrblock cfrpreset cfrop entdispfieldui
