**dbxfsd** is a simple rc(8) daemon for Rian Hunter's [dbxfs],
a user-space file system for Dropbox.

[dbxfs]: https://github.com/rianhunter/dbxfs/

### Installation

```sh
$ su
# make install
```

### Configuration

To run the daemon at startup, add `dbxfsd=` to your `/etc/rc.conf.local`.
Any specified flags will be passed onto dbxfs.

For example, I use the following flags:

```sh
dbxfsd_flags="-o uid=1000,allow_other"
```
