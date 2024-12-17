# Linux Commands

## APT

### Remove | Purge | dpkg
* dpkg spefific package
```shell
sudo apt list --installed | grep "<package-name>"

sudo dpkg -l | grep "<package-name>" | cut -d " " -f 3 | xargs sudo dpkg --purge

sudo apt autoremove -y
```

## SSH

### X11Config

* control mouse via ssh
```shell
ssh -XC htpc x2x [-nomouse|-east|-west] -to :0.0
```

