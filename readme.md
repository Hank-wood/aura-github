# AuraHub example

## Installing

First, clone this repository :

    git clone git://github.com/sbellity/aura-github.git

Create a Github App 
    
    open https://github.com/settings/applications/new

With 

Main Url:       `http://localhost:8000/`
Callback Url:   `http://localhost:8000/auth.php`

Then serve this repo via apache or start a php dev server : 

    php -S localhost:8000 -t public

## Hacking

Install [node.js](http://nodejs.org) (Only used for building the app, not needed for deployment)

[grunt-cli](https://github.com/gruntjs/grunt-cli) as a global module.

    [sudo] npm install grunt-cli -g
    [sudo] npm install bower -g

then install grunt and it's modules in the project's folder.

    cd aura-github/
    npm install
    bower install

To rebuild the dependencies

    grunt build