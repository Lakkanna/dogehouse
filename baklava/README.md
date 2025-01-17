# Dogehouse for Desktop (Baklava)

This is the desktop application for Dogehouse.
It uses ElectronJS as a wrapper for [dogehouse.tv](https://dogehouse.tv) and adds other native capabilities.

## Features

- Notifications
- System tray
- Global keybinds
- Splash screen

## How to run
- Run `yarn install`
- Ensure [Rust](https://www.rust-lang.org/learn/get-started) is installed
- Install `nj-cli` by running `cargo install nj-cli`
- Run `yarn build:globkey`
- Run `yarn start`
- *(Optional)* Run `yarn build:%YOUR_PLATFORM_CODE%` and install the app from the build *(located in `/builds`)*

If you encounter any errors while building please create a new issue for it or ask for help on the [Discord](https://discord.gg/wCbKBZF9cV0).

## Using hot reload

The electron wrapper has the capability for hot reloads during development.
You can run the app in hot reload mode using `npm run dev`.

While in hot reload mode, any time you save changes to a `ts` file, the electron app will recompile and relaunch itself.
To exit hot reload mode, use `Ctrl+C` in the console. This will however, leave the current app window open, so be sure to close that also, as it will no longer have access to hot reload.
