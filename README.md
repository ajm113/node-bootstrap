# Node Bootstrap
*Simple bootstrap Vagrantfile for setting up simple Node workbench.*

## Install

- Clone project directory somewhere.
- Run `$ vagrant up` in the root directory.
- Delete this project's .git folder.
- Start working away! :D

## Installs

- Node 7.x
- npm 4.x.x
- gulp.js
- bower

## Notes

For windows users when running `$ npm install` or `$ npm i` please use `--no-bin-links`!
Windows symlinks don't play nice with Linux symlinks npm uses, specially when
using Vagrant.
