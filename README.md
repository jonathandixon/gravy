# Gravy

Pour it on your shell to make it taste better.


## Overview

This is just a collection of scripts that make life a little easier.

## Installation

Clone this project and add the `bin` directory to your `PATH`.

    echo "export PATH=$PATH:~/path/to/gravy/bin" >> ~/.bashrc

Make sure the `gravy` script is executable.

    chmod 755 bin/gravy

## Usage

    gravy {COMMAND} [{OPTIONS}]

## Commands

- `tunnel` - Kill/Create an SSH Tunnel.

## Configurations

Some gravy commands support predefined configurations. For the ones that do
there should be a example in the `config/{command}` directory. To create
configuration just copy the example file to a file with the desired
configuration name in the `config/{command}` directory.

For example let's say we want a predefined ssh tunnel:

    cp config/tunnel/example config/tunnel/train

Then just edit the configuration and use like this:

    gravy tunnel train
