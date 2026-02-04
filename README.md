| Name                       | Status                                                       |
| -------------------------- | ------------------------------------------------------------ |
| Pipeline for `main`      | [![pipeline status](https://gitlab.3h-co.de/private/project/badges/main/pipeline.svg)](https://gitlab.3h-co.de/private/project/-/commits/main) |
| Pipeline for `production`      | [![pipeline status](https://gitlab.3h-co.de/private/project/badges/production/pipeline.svg)](https://gitlab.3h-co.de/private/project/-/commits/production) |
| Code coverage for `main` | [![coverage report](https://gitlab.3h-co.de/private/project/badges/main/coverage.svg)](https://gitlab.3h-co.de/private/project/-/commits/main) |

| Name                       | Status                                                       |
| -------------------------- | ------------------------------------------------------------ |
| Pipeline for `main`        | ![pipeline status for main](https://github.com/iBrotNano/project/actions/workflows/build.yml/badge.svg) |
| Pipeline for `production`  | ![pipeline status for main](https://github.com/iBrotNano/project/actions/workflows/build.yml/badge.svg?branch=production) |
| Code coverage for `master` | [![coverage report](https://gitlab.3h-co.de/private/project/badges/master/coverage.svg)](https://gitlab.3h-co.de/private/project/-/commits/master) |

[[_TOC_]]

# Readme

Maintainer: <marcel@3h-co.de>

Version: 4.7.1.1

## What is it?

What is the project about?

## File an issue

You can file an issue here in GitHub/GitLab. Please use the issue templates "bug report" for bugs and "feature request" for missing features. The other issue types are for internal planning and documentation. Those issue types are forms which will lead you through the reporting process.

## Documentation

You will find all documents written while the development of the project in the Wiki at [Uri to the wiki].

The api documentation will be published at [Uri to the api docs].

## Development

### Clone the project

You can clone the project with:

```bash
git clone https://username@repository.uri/project.git
```

### Contribute

Your help is welcome. File an issue or even commit code. You can fork this project and make pull requests if you have cool new features or bug fixes.

### Environment

A bunch of tools are used to create the application, run it's tests and manage it's dependencies. Here is a short briefing about which tools are used and how to set up your environment to work with the source code.

#### Git LFS

https://git-lfs.github.com/

The project uses Git LFS to manage large binary files.

To add new types of files which should be managed by Git LFS you can add them to *.gitattributes* by command line:

```bash
git lfs track "*.format-extension"
```

#### NuGet

Regular NuGets are obtained from the NuGet Repository. This is managed and hosted by Microsoft. It is already preconfigured in Visual Studio. No further steps are necessary.

Own NuGets are hosted in a dedicated Nexus instance. This must be configured in Visual Studio.

1. **Strg + Q**
2. Search for **Package Sources**
3. Add a new source using the plus symbol
4. Enter **Nexus** as name
5. Add the source URI
6. Visual Studio may ask for the credentials when the URL is called and save them locally so that they do not have to be entered again.

The build of a NuGet can be set in the project settings.

#### Configuration of the project

A step by step description of how to set up the application to run locally for development and testing purposes.

## Known Issues

A list of known issues and workarounds.