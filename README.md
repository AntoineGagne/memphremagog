# memphremagog

## Getting started

To prepare the build environment, the script provided by Poky must be sourced:

```sh
source ./layers/third-party/poky/oe-init-build-env
```

All the following commands will assume that the script has been sourced.

### Layers

The `layers` directory has two subfolders: 

- `first-party`: For layers that are managed by us;
- `third-party`: for layers that are not managed by us (i.e. `poky`).

To add new layers, the following command can be used:

```sh
bitbake-layers add "${path_to_new_layer}"
```

To see the current layers, the following command can be used:

```sh
bitbake-layers show-layers
```
