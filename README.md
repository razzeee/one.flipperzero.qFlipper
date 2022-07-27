# qFlipper Flatpak

## First checkout

Make sure to initialize the git submodule:

```
git submodule update --init --recursive
```

## Building

```
flatpak-builder build-dir --user --ccache --force-clean --install one.flipperzero.qFlipper.yml
```

Then you can run it via the command line:

```
flatpak run one.flipperzero.qFlipper
```

or just search for the installed app on your system
