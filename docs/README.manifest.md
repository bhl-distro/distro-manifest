# Distro Core Repository distro-manifest

This repository contains repo manifest files for the Distro Core distribution. The
distribution is based on Yocto tools to create a specialized Linux distro. The current
distribution available with the manifest [default.xml](./default.xml).

*   [Yocto Releases](https://wiki.yoctoproject.org/wiki/Releases)

The development tasks manual is a invaluable resource to understanding the intricacies of using
the project for creation of specialized Linux distributions.

*   [Yocto Project Development Tasks](https://docs.yoctoproject.org/dev-manual/index.html)

Repo is a tool built on top of Git. Repo helps manage many Git repositories, does the uploads to
revision control systems, and automates parts of the development workflow. Repo is not meant to
replace Git, only to make it easier to work with Git. Git projects are captured into XML files
for use by the repo tool. This allows for many different configurations and revisions to be
captured into one location.

*   [Repo Tool information](https://android.googlesource.com/tools/repo)


# Manifests

Manifests are descriptions of the repositories that are to be included in the build. The
repositories may be from the same organization or from different organizations. The manifest
files are stored in the .repo/manifests path upon initialization by the repo command. The
presence of a repository in layers/* does not automatically add it to the bitbake layers.


## Manifest Descriptions

Repository manifests

| Manifest | git refs | LTS | EOL | Description |
| --- | --- | --- | --- | --- |
| default.xml | HEAD | | | Soft link to current manifest |
| [distro-head-kirkstone.xml](./distro-head-kirkstone.xml) | HEAD | Yes | 2026-04 | Development, Yocto Kirkstone (4.0) |
| [distro-head-scarthgap.xml](./distro-head-scarthgap.xml) | HEAD | Yes | 2028-05 | Development, Yocto Scarthgap (5.0) |
| distro-refs-*.xml | commit-id | | | Development CI/CD |
| remotes*.xml | | | | Repo Remotes Definitions |
| upstream-head*.xml |  | | | Mirrors from Upstream Definitions |
