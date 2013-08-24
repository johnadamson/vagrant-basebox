## About
Looking for a basic box to use with Vagrant?

- [Vagrant](https://github.com/mitchellh/vagrant/wiki/Available-Vagrant-Boxes)
- [Ubunutu Cloud Images](http://cloud-images.ubuntu.com/vagrant/)

What to build your own? This collection of tools will help preseed a basic Ubuntu box.

## Usage

```sh
./build.sh
```

# Requirements

### mkisofs

Install [homebrew](http://mxcl.github.com/homebrew/), then:

```sh
brew install cdrtools  
```

### libarchive

If you are running Mac OS 10.7+ and notice untarring the ISO silently fails:

```sh
brew tap homebrew/dupes
brew install libarchive
```

You can preemptively determine if you need libarchive by running

```sh
tar --version
```

If you have version 2.8.3, and you run Lion, you will likely need to install
libarchive.

