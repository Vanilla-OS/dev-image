# Vanilla OS Dev Image

Containerfile for building a Vanilla OS Development Kit Image.

> [!NOTE]
> This image is meant to be used for development purposes only.

## Build

You need the [Vib](https://github.com/vanilla-os/Vib) tool to generate the Containerfile.

```bash
vib build recipe.yml
podman image build -t vanillaos/dev .
```
