Cordova Box
=============================

Ionic Box is a ready-to-go hybrid development environment for building mobile
apps with Cordova and Android. Cordova Box was built to make it easier
for developers to build Android versions of their app, and especially for
Windows users to get a complete dev environment set up without all the
headaches.

Cordova Box is a fork of [Ionic Box](https://github.com/driftyco/ionic-box).

### Installation


To install, download and install [Vagrant](https://www.vagrantup.com/downloads.html) for your platform, then download and install [VirtualBox](http://virtualbox.org/).

Once Vagrant and VirtualBox are installed, you can download the latest release of this GitHub repo, and unzip it. `cd` into the unzipped folder and run:

```bash
$ vagrant up
$ vagrant ssh
```

The username for vagrant is `vagrant` and the password is `vagrant`.

This will download and install the image, and then go through the dependencies and install them one by one. `vagrant ssh` will connect you to the image and give you a bash prompt. Once everything completes, you'll have a working box to build your apps on Android.

### Connected Android Devices

The image also has support for connected USB Android devices. To test whether devices are connected, you can run (from the box):

```bash
$ adb devices
```

If that does not work, or shows `????? permissions`, then run:

```bash
adb kill-server
adb start-server
```
