# User Bundle

A new Symfony bundle for basic user management.

[![Latest Stable Version][packagist:img]][packagist]

# Installation

```bash
composer require msgphp/user-bundle
```

# Configuration

```php
<?php
// config/packages/msgphp_user.php

use MsgPhp\User\User;
use Symfony\Component\DependencyInjection\Loader\Configurator\ContainerConfigurator;

return function (ContainerConfigurator $container) {
    $container->extension('msgphp_user', [
        'class_mapping' => [
            User::class => \App\Entity\User::class,
        ],
    ]);
};
```

## Feeling Lazy?

```bash
composer require maker --dev
bin/console make:user:msgphp
```

# Documentation

- Read the [bundle documentation](https://msgphp.github.io/docs/cookbook/user-bundle/installation/)
- Try the Symfony [demo application](https://github.com/msgphp/symfony-demo-app)
- Get support on [Symfony's Slack `#msgphp` channel](https://symfony.com/slack-invite) or [raise an issue](https://github.com/msgphp/msgphp/issues/new)

# Contributing

This repository is **READ ONLY**. ~~Issues and pull requests should be submitted in the
[main development repository](https://github.com/msgphp/msgphp).~~

For some reasons original msgphp/* repositories was was marked as archived by an administrator on Jun 29, 2023. It is no longer maintained.
Since we are using this bundles in production - we created mirror [msgphp2/*](https://github.com/msgphp2) 
Feel free to use and contibute!

[packagist]: https://packagist.org/packages/msgphp/user-bundle
[packagist:img]: https://img.shields.io/packagist/v/msgphp/user-bundle.svg?style=flat-square
