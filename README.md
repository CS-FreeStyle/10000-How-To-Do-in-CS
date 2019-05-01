# 10 000 How-To-Do in CS
Welcome to contribute to this repository! Since editing this file would take some time(ajusting the format), you can also contribute by submitting an issue with problem and solution.

# Contents:
- [How to install Unity on Ubuntu16.04](#how-to-install-unity-on-ubuntu1604)
- [How to check Nvidia graphics card utilization](#how-to-check-nvidia-graphic-card-utilization)
- [libGLU.so.1](#libgluso1)
- [Extract ISO file](#how-to-extract-iso-files-on-linux)

## How to install Unity on Ubuntu16.04?

1.Install dependences:

	$ sudo apt-get -f install libpq5 lib32gcc1 lib32stdc++6 libc6-i386 nodejs node-abbrev node-ansi-color-table node-ansi node-archy node-block-stream node-fstream node-fstream-ignore node-github-url-from-git node-glob node-graceful-fs node-inherits node-ini node-lockfile node-lru-cache node-minimatch node-mkdirp node-gyp node-nopt node-npmlog node-once node-osenv node-read node-read-package-json node-request node-retry node-rimraf node-semver node-sha node-slide node-tar node-underscore node-which node-form-data node-node-uuid node-mime node-forever-agent node-tunnel-agent node-json-stringify-safe node-cookie-jar node-qs libjs-node-uuid node-sigmund libjs-inherits gyp node-mute-stream node-normalize-package-data node-combined-stream node-async node-delayed-stream

2.Install gdebi, which can install the neccessary depences when you install xx.deb packages:

	$ sudo apt-get install gdebi

3.Download the latest eversion:

	https://forum.unity.com/threads/unity-on-linux-release-notes-and-known-issues.350256/

4.Install Unity using gdebi:

	$ sudo gdebi unity-editor_amd64-2017.2.0xb6Linux.deb
Now, search your computer for "Unity" icon and click to lauch unity.

## How to check Nvidia graphic card utilization?
	$ nvidia-smi
	$ watch -n 1 nvidia-smi
	
## libGLU.so.1
Problem: error while loading shared libraries: libGLU.so.1?

	$ sudo apt-get install libglu1-mesa:i386

## How to extract ISO files on Linux?

1. We can use 7z to decompress a iso file.

2. We can use this command: `cmake -E tar xf filename.iso`

3. Use FUSE

Mounting
To mount an image:

$ fuseiso image directory
The destination mount point must be writable and have no other mounted files or devices to it.

Run fuseiso -h for all the available options.

Unmounting
To unmount the image:

$ fusermount -u directory
