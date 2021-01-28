# Solid Community Server recipes
This repository contains example configurations
for the [Solid Community Server](https://github.com/solid/community-server/),
to get you started quickly.

You can launch the Solid Community Server with the following user interfaces:
- [Mashlib Data Browser](https://github.com/solid/mashlib)
- [Penny](https://forum.solidproject.org/t/new-developer-tool-app-penny/3837)


## Installing the recipes
```shell
# Load the configurations to your device
git clone https://github.com/solid/community-server-recipes
cd community-server-recipes

# Pick the configuration of your choice, and install its dependencies
cd mashlib   # or penny
npm ci
```


## Starting the server from a recipe

### Mashlib
The Mashlib configurations are in the `mashlib` folder.

```shell
# Start the server with your documents folder as the root container
npx community-solid-server -c config-mashlib.json -f ~/Documents/

# Start the server in development mode (authenticated as a specific user)
npx community-solid-server -c config-mashlib-dev.json -f ~/Documents/
```

### Penny
The Penny configurations are in the `penny` folder.

```shell
# Start the server with your documents folder as the root container
npx community-solid-server -c config-penny.json -f ~/Documents/
```
