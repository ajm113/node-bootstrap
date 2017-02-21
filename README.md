# Node Bootstrap
*Simple bootstrap Vagrantfile for setting up simple Node workbench.*

## Install

I assume you are somewhat familiar with Vagrant. If not you can read more
about it here >>> https://www.vagrantup.com/docs/getting-started/

- Clone project directory somewhere.
- Run `$ vagrant up` in the root directory.
- SSH at `192.168.33.11`. (You may change this in `Vagrantfile`!)
- Delete this project's .git folder. (*If you want to work in the root directory*)
- Start working away! :D

## Default Installations In VM

- Node 7.x
- npm 4.x.x
- gulp.js
- bower

## Notes

For windows users when running `$ npm install` or `$ npm i` please use `--no-bin-links`!
Windows symlinks don't play nice with Linux symlinks npm uses, specially when
using Vagrant.

The default `private_network` is `192.168.33.11` if you feel this will collide
with other VMs or devices, you may change this.
