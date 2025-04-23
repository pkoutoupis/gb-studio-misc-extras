# gb-studio-misc-extras
Miscellaneous extra features and plugins for GB Studio.

Author: Petros Koutoupis (<petros@petroskoutoupis.com>)

## Patches

The patches are designed to for the GB Studio engine which can be exported
for your project from within the software development kit.

To apply, navigate to the project's root directory and:

```console
$ patch -p0< new-feature.patch
```

## Plugins

To install the plugin, copy the plugin's parent directory into the `plugins/`
subdirectory of your project. Then reload the assests or reload your project
in GB Studio.

### Dependencies

The `Advanced Dialogue` plugin requires the following patch to enable close
with the press of Start: `gb-studio-<version>_engine-add-start-wait-flag.patch`

The `Edit Actor Active Index` plugin requires the following patch to properly
use the Set Actor Active Index: `gb-studio-4.1.3_engine-set-actor-active-index.patch`

## Additional Notes

The `Advanced Dialogue` plugin is a fork of a now depracated plugin of the
same name originally developed and distributed by `pau-tomas`. It has been
modified to support "close with the press of the Start button" and to adjust
open/close speeds from the user interface. Original project: `gb-studio-plugins`

The `Edit Actor Active Index` plugin is a modified condensed and minimal port of
Mico27's plugin of the same name. It is used to render actors in a specific order.
Sort of like defining z-index of actors on screen.
