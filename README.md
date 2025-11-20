# BlueBuild Template &nbsp; [![bluebuild build badge](https://github.com/blue-build/template/actions/workflows/build.yml/badge.svg)](https://github.com/blue-build/template/actions/workflows/build.yml)

See the [BlueBuild docs](https://blue-build.org/how-to/setup/) for quick setup instructions for setting up your own repository based on this template.

After setup, it is recommended you update this README to describe your custom image.

## Installation

> [!WARNING]  
> I only support Clean installing this system
>
> DO NOT ATTEMPT TO USE rpm-ostree rebase TO ATTEMPT TO MIGRATE FROM ANOTHER rpm-ostree BASED SYSTEM
>
> YOU WILL RUN INTO PROBLEMS IF YOU DO THAT

There's only one version of this system and that's the latest version

upgrades are automatic and happen daily

this is intended for thin clients so nothing that could be easily broken via an update should be deployed to systems running this

The `latest` tag will automatically point to the latest build. That build will still always use the Fedora version specified in `recipe.yml`, so you won't get accidentally updated to the next major version.

## ISO

Coming Soon

## Verification

These images are signed with [Sigstore](https://www.sigstore.dev/)'s [cosign](https://github.com/sigstore/cosign). You can verify the signature by downloading the `cosign.pub` file from this repo and running the following command:

```bash
cosign verify --key cosign.pub ghcr.io/blue-build/template
```
