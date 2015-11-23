# Simple Node

## 1. General
This section will teach you how to install the current Node.js version, how to use the awesome package manager, and what tools to use for code management, deployment, etc.

#### Installation
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

    node -v

and you should see the installed Node.js version.


## 2. Tools
---
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
