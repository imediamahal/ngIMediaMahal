Part-A: Node, npm and  Angular Setup: 
    I had the latest nodejs from https://nodejs.org/

        Check Node version: node -v : v20.10.0

        Check NPM version: npm -v: v10.2.3

        which is not compatible with Angular CLI 15 , the latest version that is compatible with
        Material (Check Angular / Nodejs compatibility here: https://angular.io/guide/versions)

        So I end up downloading the v18 thru this link https://nodejs.org/en/blog/release/v18.12.0

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

        if github commit shows you have 700+ updates, add this line to your .gitignore
            # Other miscellaneous C:Userssvisunodejsnpm-cache
            C:Userssvisuvnodejsnpm-cache/
        and run this in your terminal to clear already committed cache if any 
            git rm -rf C:Userssvisuvnodejsnpm-cache/


    Make sure every thing works by running ng serve -o 

Part-B: Angular Material Setup:

    Visit Materials Getting Started documentation here: https://material.angular.io/guide/getting-started

    Using ng add @angular/material install material in your project.

    It will install  @angular/material@15.2.9 in your project folder.

    Once installed make sure yor app is still functional at http://localhost:4200 
