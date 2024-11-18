<img src="https://avatars.githubusercontent.com/u/14262490?s=66" alt="[Solid Logo]" align="right" />

# 🍱 Community Solid Server recipes
This repository contains example configurations
for the [Community Solid Server](https://github.com/CommunitySolidServer/CommunitySolidServer),
to get you started quickly.

You can launch the Community Solid Server with the following user interfaces:
- [Mashlib Data Browser](https://github.com/SolidOS/mashlib)
- [Penny](https://forum.solidproject.org/t/new-developer-tool-app-penny/3837)


## ⚙️ Installing the recipes
```shell
# Load the configurations to your device
git clone https://github.com/CommunitySolidServer/Recipes
cd Recipes

# Pick the configuration of your choice, and install its dependencies
cd mashlib   # or penny
npm ci --omit=dev
```


## 🚀 Starting the server from a recipe

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

## 📜 Customizing the recipes
The configurations provided here are just one possible combination of CSS features.
You can use the following links to generate alternative configurations
that also include the necessary statements for the relevant interfaces:
  * [Mashlib](https://communitysolidserver.github.io/configuration-generator/v7/?config=https://raw.githubusercontent.com/CommunitySolidServer/Recipes/main/mashlib/config-mashlib.json&removeImports=%22util/index%22)
  * [Penny](https://communitysolidserver.github.io/configuration-generator/v7/?config=https://raw.githubusercontent.com/CommunitySolidServer/Recipes/main/penny/config-penny.json&removeImports=%22util/index%22)
