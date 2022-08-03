# qFlipper Flatpak

## First checkout

Make sure to initialize the git submodule:

```
git submodule update --init --recursive
```

## Udev rules

You will need to have the following udev rules from qFlipper installed:
https://github.com/flipperdevices/qFlipper/blob/dev/setup_rules.sh

## Building

```
flatpak-builder build-dir --user --ccache --force-clean --install one.flipperzero.qFlipper.yml
```

Then you can run it via the command line, be sure to allow the udev access:

```
flatpak run --filesystem=/run/udev:ro one.flipperzero.qFlipper
```

or just search for the installed app on your system
