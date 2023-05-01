# Libpd RtAudio Example.

This repository shows how to use libpd embedded in a cpp program using the RT audio.

The pd Patch is a simple ring modulator which receives the modulation frequency from cpp. The patch also comunicates with the cpp program  via a `send` object with the label `cursor`.

### Download the repository
Since this repository depends on [libpd](https://github.com/libpd/libpd) (as a submodule) you cannot download it as zip.
Open a terminal and run:
```
$ git clone --recurse-submodules https://github.com/ddgg-el/libpd_cpp.git
```
If you didn't use the `--recurse-submodules` flag, you can always update the submodules as follows:
```
$ git submodule update --init --recursive
```

### Building the software
It should be enough to run:
```
$ cd <path/to/this/repo>
$ make
```
This command should build both `libpd` and all the files inside the src folder.

### Troubleshooting
First of all you need to understand whether you have problems compiling `libpd`or this project.
You could infact decide to build only libpd. From the project folder:
``` 
$ cd libpd
$ make
```
If you are facing errors or for more advanced building options please refer to the [libpd Documentation](https://github.com/libpd/libpd#building-libpd)

If the errors are produced by this project get in touch!