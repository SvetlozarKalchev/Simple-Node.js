# Simple Node

## 1. Installation
First thing's first - let's install the last stable Node.js version. The best way to ensure you get the most current release if you are running OSX or Linux is to download the binary from the official website and manually install it. However, using a package manager is much easier and will also do the job.

#### Windows
Download and run the official windows installer available on [nodejs.org](https://nodejs.org/en/#download).

#### OSX
There are 3 ways to install Node on OSX. You can use a package manager like this:

    brew install node
  or

    port install nodejs

You can also download the installer from the [official site](https://nodejs.org/en/#download).

#### Linux (Debian & Ubuntu)
I wouldn't recommend using your distro's official package manager to install node, because the available package will most likely be really old. Here's how to to do it properly:

      curl -sL https://deb.nodesource.com/setup_5.x | sudo -E bash -
    sudo apt-get install --yes nodejs

You also need to link the installed files to the node binary, so you can use **node** from the command line.

    sudo ln -s /usr/bin/nodejs /usr/bin/node


---
No matter what OS you're running, verify that everything runs as it should after the installation. Simply do:

    node -v && npm -v

and you should see the installed Node.js and npm versions.


## 2. Tools

#### npm
The Node ecosystem has awesome tools that make your life as a developer really easy. Perhaps the most essential one you are going to need is **npm** - node's package manager.

Much like in Rails, the de-facto way of managing dependencies in Node is through modules - you download and install different software packages either locally or globally and then you use them in your code or from the command line All this is achieved with **npm**. Writing your own custom modules is really easy and actually a good practice if you have some functionality that can easily be separated. After finishing your package simply use **npm** to upload it in the [official repository](https://www.npmjs.com/).

To install a node package open your shell and simply write:

    npm install [package_name]

This will install the chosen module in the current directory, e.g. locally. If you want to use the package in other projects without repeatedly installing it, choose the --global option on the first run.

    npm install -g [package_name]

Removing packages is really easy:

    npm uninstall [package_name]

or if the package is global

    npm uninstall -g [package_name]

----
### bower
While npm will manage our node modules, which we use on the back-end, we don't have anything doing the same for our front-end stuff. Fortunately, the good guys from Twitter wrote bower



  npm, bower, installing packages, .gitignore setup

2. Code Organization

  2.1 Directory Structure

    research different structures

  2.2 Modules

  what is module.exports?

  what kind of module exports patterns are there

3. Functions

  3.1 Scope and Asynchronious Operations

  types of scope in JS, how arguments are passed, caching this, ES6 arrow functions

  3.2 Error Handling

  types of errors according to Joyent's Guide

4. Classes

  4.1 Patterns

    prototypal inheritance and es6
