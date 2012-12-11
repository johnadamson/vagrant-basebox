### This is a fork of [vagrant-ubuntu-precise-64](https://github.com/cal/vagrant-ubuntu-precise-64)


Note: If you are running OS X 10.7+ and notice untarring the ISO silently
fails:

    brew tap homebrew/dupes
    brew install libarchive

You can preemptively determine if you need libarchive by running:
  
    tar --version

If you have version 2.8.3, and you run Lion, you most likely will need
to install libarchive.


## About

This script will: 

 1. download the Ubuntu 12.04 alternate server, 64bit iso
 2. ... do some magic to turn it into a vagrant box file
 3. output package.box 

## Usage

    ./build.sh

This should do everything you need. If you don't have 
mkisofs, install [homebrew](http://mxcl.github.com/homebrew/), then:

    brew install cdrtools

### Ben's notes

Forked Carl's repo, and it sort of worked out of the box. Tweaked 
office 12.04 release: 

 - Downloading 12.04 final release. (Today as of this writing)
 - Checking MD5 to make sure it is the right version
 - Added a few more checks for external dependencies, mkisofs
 - Removed wget, and used curl to reduce dependencies
 - Added more output to see what is going on
 - Still designed to work on Mac OS X :)
    ... though it should work for Linux systems too (maybe w/ a bit of porting)

### Carl's original README

Decided I wanted to learn how to make a vagrant base box.

Let's target Precise Pangolin since it should be releasing soon, I said.

Let's automate everything, I said.

Let's do it all on my macbook, I said.

Woo.
