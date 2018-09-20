linkemon
===========

A tiny wrapper script built around [nodemon](https://github.com/remy/nodemon) that will automatically 
watch all your linked `node_module`s while ignoring all the rest. As the name says, 
it should solve your `nodemon` problems when you use a lot linked modules, such as when 
having monorepos ([Lerna](https://github.com/lerna/lerna), Yarn Workspaces, etc.).

## Install
```
# make sure you have nodemon already installed
npm install -g nodemon

npm install -g linkemon 
```

## Usage

Use the script as you would normally use `nodemon`. Behind the scenes the script will add any 
linked module in the `./node_modules` directory to the watchlist. For example:

```
linkemon -V server.js
```
