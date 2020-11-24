# Vagrant & VM Provisioning

## Provisioning
- Derived from providing and supplying something e.g. food provisions
- In this context it will be providing our machines with instructions, variables
, files, and folders
- This allows us to set up a virtual machine in a specific state when turned on

## Sending files into the VM
- Can include ```config.vm.synced_folder "src/folder", "/destination/folder"```
in the Vagrantfile to sync a folder between your host and guest machine
- The first parameter is the path to the directory in the host machine (it will
  automatically be relative to the root unless specified otherwise)
- The second parameter is where the folder will be created in the guest machine
- This is NOT copying in, it is SYNCING
- Therefore, if we change something on one machine, it will change the file on
both

## Ruby's testing framework is rpsec
- rspec needs to be installed
- if bundler isn't installed run ```gem install bundler```
- go to folder with Gemfile
- run ```bundle```
- run ```rake spec```

## Bundler and gems vs pip and packages
- Gems are packages in Ruby or dependencies
- Bundler is Ruby's package manager
- Gemfile keeps a list of dependencies to be installed
- To install gems from the Gemfile, you run: ```bundle install```
- JS package manager is npm (node package manager)
  - after version 6 it comes pre loaded with npm
- Ubuntu package manager is apt-get
