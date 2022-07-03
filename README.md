# TeXbld templates

These are free-to-use texbld templates that you can either directly use or
inherit in your images. It serves as an example for how to structure a
multi-config texbld image repository.

## Scaffolding a Project (v0.2)

The vanilla template:

```sh
texbld generate project github:texbld/templates#master (directory)
```

The markdown template:

```sh
texbld generate project github:texbld/templates#master -c md.toml (directory)
```

The essay template:

```sh
texbld generate project github:texbld/templates#master -c essay.toml (directory)
```

## Scaffolding a Project (v0.1)

The vanilla template:

```sh
texbld generate github texbld templates --rev master (directory)
```

The markdown template:

```sh
texbld generate github texbld templates --rev master -c md.toml (directory)
```

The essay template:

```sh
texbld generate github texbld templates --rev master -c essay.toml (directory)
```
