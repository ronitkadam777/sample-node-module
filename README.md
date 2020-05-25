# sample-node-module
This repository consist of a simple node module which is meant to be reused by consumer application.

# Pre-requisities to host the node module (One time setup)
1. Either publicly host the node module or use a private npm proxy like Verdaccio.
( I have hosted a Verdaccio instance on http://64.xxx.xxx.xxx/ )
2. Point npm client to Verdaccio by running command: ```npm set registry http://64.xxx.xxx.xxx/```

# On Node Module Project: Everytime the node module needs to be published
3. To update the version run ```npm version patch```. 
(Replace ```patch``` with ```major``` or ```minor`)
4. Publish to Verdaccio by running ```npm publish```

# On Consumer Project
5. Install the node module xyz ```npm install xyz```
