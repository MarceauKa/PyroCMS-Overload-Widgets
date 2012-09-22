# PyroCMS Overload widgets

* Version: 1.0

## Team

* [Marceau Casals](http://www.akibatech.fr/)

## Description

This Widgets.php replacement allows you to overload display.php from widgets views in your theme.

## Licence

WTFPL - Do What The Fuck You Want To Public License.

DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
Version 2, December 2004

Copyright (C) 2004 Sam Hocevar <sam@hocevar.net>

Everyone is permitted to copy and distribute verbatim or modified
copies of this license document, and changing it is allowed as long
as the name is changed.

DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION

0. You just DO WHAT THE FUCK YOU WANT TO.

## Compatibility

Tested and approved with PyroCMS 2.1.4

## Installation

Just replace system > cms > modules > widgets > libraries > Widgets.php by the equivalent provided here.

## What you can do?

This modification works with :
* A stand-alone widget (placed in the PyroCMS widget directory : system / cms / widgets)
* A module's widget (simply, a widget provided by a module : system / cms / modules / {module-name} / widgets)

## How can you do?

The widget structure is generally like that :
* {widget-name}/
    * {widget-name}.php
    * views/
        * display.php
        * form.php

Create a folder named "widgets" in your current theme's view folder.

Ex :
* addons > {site-ref} > themes > views > widgets
* shared_addons > themes > views > widgets

Now, just create a new php file named by the module's name you want to overload.

Ex :
I want to overload the Navigation widgets view. Its front-end view is stored in views > display.php.
I have to copy this display.php in my theme's widget folder, and rename it by the widget's name, like that : navigation.php.

## Note

I apologize for my poor english...