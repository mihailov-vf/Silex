[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fmihailov-vf%2FSilex.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2Fmihailov-vf%2FSilex?ref=badge_shield)

Silex, a simple Web Framework
=============================

Silex is a PHP micro-framework to develop websites based on `Symfony
components`_:

.. code-block:: php

    <?php

    require_once __DIR__.'/../vendor/autoload.php';

    $app = new Silex\Application();

    $app->get('/hello/{name}', function ($name) use ($app) {
      return 'Hello '.$app->escape($name);
    });

    $app->run();

Silex works with PHP 5.5.9 or later.

Installation
------------

The recommended way to install Silex is through `Composer`_:

.. code-block:: bash

    composer require silex/silex "~2.0"

Alternatively, you can download the `silex.zip`_ file and extract it.

More Information
----------------

Read the `documentation`_ for more information and `changelog
<doc/changelog.rst>`_ for upgrading information.

Tests
-----

To run the test suite, you need `Composer`_ and `PHPUnit`_:

.. code-block:: bash

    composer install
    phpunit

Community
---------

Check out #silex-php on irc.freenode.net.

License
-------

Silex is licensed under the MIT license.

.. _Symfony components: http://symfony.com
.. _Composer:           http://getcomposer.org
.. _PHPUnit:            https://phpunit.de
.. _silex.zip:          http://silex.sensiolabs.org/download
.. _documentation:      http://silex.sensiolabs.org/documentation


## License
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fmihailov-vf%2FSilex.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2Fmihailov-vf%2FSilex?ref=badge_large)