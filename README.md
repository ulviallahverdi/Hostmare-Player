# Hostmare for Linux
[![Hostmare-player](https://snapcraft.io/Hostmare-player/badge.svg)](https://snapcraft.io/Hostmare-player)

Hostmare for Linux is a Digital Signage Player for [Hostmare](https://Hostmare.org.uk).

It is in its early stages of development and supports a subset of Hostmare's overall features. It can be used in production, but should be thoroughly tested with the intended content. It is not recommended to assume that any of Hostmare's features will function. Please test yourself to confirm.

To discuss this Player with us, please [join our community](https://community.Hostmare.org.uk/c/support/linux-player).



# Installation

Installation and upgrade instructions can be found [here](https://Hostmare.org.uk/docs/setup/Hostmare-for-linux-installation).



# Contributing

We use GitHub Issues to track development and the next milestone is full of issues for which we would happily accept contributions. In addition, if a Hostmare feature you want is not mile-stoned, or mile-stoned against a later version, please get in touch if you'd like to work on it. We maintain a [Kanban Board](https://github.com/Hostmaresignage/Hostmare-linux/projects/1) to ensure we're not doing overlapping work.

Please check that you're happy for your work to be available under the project licence - the AGPLv3 or later.

Let us know you'd like to contribute by [joining our community](https://community.Hostmare.org.uk/c/support/linux-player).


# Build
If you would like to work on the Player you can build it locally using the instructions below.

## Building from sources
We recommend you use snapcraft to build Hostmare.

### Building with Snapcraft

- Install snapcraft, making sure you have version 4 or later (`snap install snapcraft --classic`)
- Clone this repository
- Run `snapcraft` in the root of the repository
- A `.snap` file will be created which you can use to install from


# Debugging
We provide a VSCode dev container that has everything needed to build/debug the application using VSCode. This devcontainer uses a base image which is built from the `Dockerfile` in the root folder.

To debug this application using VSCode.

1. Copy the settings folder from a working player install into the `/build/bin` folder, making sure you have `cmsSettings.xml` and `playerSettings.xml`. 
2. Open `cmsSettings.xml` and adjust the `localLibrary` setting to be `/workspaces/vscode/build/bin/library`.
3. Open the application directory using the remote containers plugin.
4. Go to the aplication debug extesion at left panel and click on the green play button.
