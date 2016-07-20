# alps_manifest

Installing Repo
````bash
curl https://storage.googleapis.com/git-repo-downloads/repo > ~/bin/repo
chmod a+x ~/bin/repo
```

To download ALPS
````bash
repo init -u git://github.com/emvirt/alps_manifest.git -b master
```
Then to sync up:
````bash
repo sync -j4
```

To download ALPS for LET-V sdcard experimental
````bash
repo init -u git://github.com/emvirt/alps_manifest.git -b master -m letv.xml
```
Then to sync up:
````bash
repo sync -j4
```

Git projects information
- alps_root: others (userspace program, test scritps, ...)
  * branches: master(alps), letv(alps for LET-V sdcard experimental)
- alps_linux
  * alps branches: master/secure, master/normal
  * alps for LET-V: letv/secure, letv/normal
- alps_monitor
  * branch: master(alps), letv(alps for LET-V)
- alps_u-boot
  * alps branches: master/secure, master/normal
  * alps for LET-V: letv/secure, letv/normal
