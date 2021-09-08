# How to build a cross compiler

If you are interested in making your own operating system, using a cross compiler might be a good idea. You don't necessarily need to, but sometimes it is the only way to prevent some weird bugs, like the ones that will happen once you need to call global objects (in case you are using c++).

## Installing the dependencies

### Linux

On a debian-based distro, all you need to do is:
```
sudo apt-get install bison flex libgmp3-dev libmpc-dev libmpfr-dev texinfo
```
You will also need build-essentials, obviously.

### Windows

Just use WSL, and the steps will be the same as the above.

---

After you have installed all the dependencies, just download the build.sh file and change the variables according to the target and the gcc/binutils version you wish to build, then you can simply run it by doing `./build.sh` and the compilation process will begin. Once that is done, enjoy your cross compiler!
