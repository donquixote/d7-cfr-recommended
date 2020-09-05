# d7-cfr-recommended
Meta package to require the most common / recommended cfr-related modules in D7.

## Installation

First install your Drupal 7 website with something like https://github.com/drupal-composer/drupal-project/tree/7.x.

    composer create-project drupal-composer/drupal-project:7.x-dev some-dir --no-interaction

Create a database, configure your local webserver, and install Drupal 7.

Then require this package:

    cd some-dir
    composer require donquixote/d7-cfr-recommended

Then enable modules with drush.

    cd web
    drush en -y entdisp listformat entdisp_example cfrblock cfrpreset cfrop entdispfieldui entity renderkit_ui

## See if it works

Create a node.
Visit `admin/structure/renderkit/preview`.
Choose and configure a display component.
Choose the theme in which to show the preview.
Hit "Show".

## Notes
Some of the components might require other modules to work.
E.g. `views` is a good idea to install, but not required for basic functionality.
