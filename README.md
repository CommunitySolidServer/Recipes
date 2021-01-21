# Solid Community Server with Mashlib
This repository contains example configurations
for the [Solid Community Server](https://github.com/solid/community-server/)
with the [Mashlib Data Browser](https://github.com/solid/mashlib)
as its default user interface.

## Installation
```shell
git clone https://github.com/solid/community-server-mashlib
cd community-server-mashlib
npm ci
```

## Usage
```shell
# Start the server with your home folder as the root container
npx community-solid-server -c config-mashlib.json -f ~/Documents/

# Start the server in development mode (authenticated as a specific user)
npx community-solid-server -c config-mashlib-dev.json -f ~/Documents/
```
