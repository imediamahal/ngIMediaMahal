Install the latest nodejs from https://nodejs.org/

Check Node version: node -v : v20.10.0

Check NPM version: npm -v: v10.2.3

This package has installed:
	•	Node.js v18.12.0 to /usr/local/bin/node
	•	npm v8.19.2 to /usr/local/bin/npm
Make sure that /usr/local/bin is in your $PATH

Check Angular CLI version: ng version
if Angular not installed, install using npm: npm install -g @angular/cli 
    for more info read: https://angular.io/guide/setup-local

My current version is: 

    Angular CLI: 14.2.13
    Node: 20.10.0 (Unsupported)
    Package Manager: npm 10.2.3 
    OS: darwin x64

I need to update to the lastest Angular version 15 that is compatible with Material (latest) using this command:
    ng update @angular/core@15 @angular/cli@15
  
    Note: if you get an error "Repository is not clean. Please commit or stash any changes before updating" you may need to add the --allow-dirty or even --allow-dirty --force in some case.