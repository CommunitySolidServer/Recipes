# Solid Community Server recipes
This repository contains example configurations
for the [Solid Community Server](https://github.com/solid/community-server/),
to get you started quickly.

You can launch the Solid Community Server with the following user interfaces:
- [Mashlib Data Browser](https://github.com/solid/mashlib)

## Installing the recipes
```shell
# Load the configurations to your device
git clone https://github.com/solid/community-server-recipes
cd community-server-recipes

# Pick the configuration of your choice, and install its dependencies
cd mashlib
npm ci
```

## Starting the server from a recipe
```shell
# Start the server with your home folder as the root container
npx community-solid-server -c config-mashlib.json -f ~/Documents/

# Start the server in development mode (authenticated as a specific user)
npx community-solid-server -c config-mashlib-dev.json -f ~/Documents/
```
