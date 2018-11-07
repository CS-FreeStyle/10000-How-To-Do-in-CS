# 10 000 How-To-Do in CS
Welcome to contribute to this repository! Since editing the format of this file takes some time, you can also contribute by submit an issue with problem and solution.

# Contents:
- [How to install Unity on Ubuntu16.04](#user-content-How-to-install-Unity-on-Ubuntu16.04)
- [How to check Nvidia graphics card utilization](#user-content-How-to-check-Nvidia-graphic-card-utilization)

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
