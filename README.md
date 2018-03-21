# PHP Mess Detector for CakePHP 3
A php mess detector ruleset file which is more compatible with CakePHP 3

## Mess Detector?
The Mess Detector project aims to automatically find problems with your code, and highlight them to improve code quality.

Find out more at [https://phpmd.org](https://phpmd.org/) or [github.com/phpmd/phpmd](https://github.com/phpmd/phpmd)

## Installation
* Copy the `phpmd.xml` file into your project root.
* Install phpmd `composer require --dev phpmd/phpmd` or globally with `composer global require phpmd/phpmd`

## Check your code on the command line
```bash
phpmd src/ text phpmd.xml --suffixes=php
```

## Run with Composer
```json
"scripts": {
    "mess": "phpmd src/ text phpmd.xml --suffixes=php"
}
```

```bash
composer mess
```

## Run as inspection in PHP Storm
In your settings, under Languages & Frameworks > PHP > Mess Detector set your 'Development environment' configuration to point to the correct executable, either in your projects 'vendor' folder, or you global folder.

Then in your settings, under Editor > Inspections > PHP add the `phpmd.xml` file to the Custom rulesets options.

[There is an official guide also](https://confluence.jetbrains.com/display/PhpStorm/PHP+Mess+Detector+in+PhpStorm)
