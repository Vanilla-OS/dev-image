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

## Verify Image Build Provenance Attestation

All the image builds/pushes are attested for build provenance and integrity using the [attest-build-provenance`](https://github.com/actions/attest-build-provenance) action. The attestations can be verified [here](https://github.com/Vanilla-OS/dev-image/attestations) or by having the latest version of [GitHub CLI](https://github.com/cli/cli/releases/latest) installed in your system. Then, execute the following command:

```sh
gh attestation verify oci://ghcr.io/vanilla-os/dev:main --owner Vanilla-OS
```
