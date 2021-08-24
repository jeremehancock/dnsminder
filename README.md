<h1><img src="https://raw.githubusercontent.com/jeremehancock/dnsminder/main/dnsminder.png" height="50" /> DNS Minder</h1>

<img src="https://raw.githubusercontent.com/jeremehancock/dnsminder/main/dnsminder-window.png" />

This simple GUI allows you to easily set up your system's DNS to use [CleanBrowsing](https://cleanbrowsing.org) or [OpenDNS FamilyShield](https://www.opendns.com/setupguide/#familyshield).

## Installed by default on UbuntuCE:

### [Check out UbuntuCE](https://ubuntuce.com/).

## Install DNS Minder on Ubuntu:

### Option 1:

DNS Minder is available in the [UbuntuCE Repo](https://github.com/jeremehancock/repo.ubuntuce.com#readme)

### Option 2:

DNS Minder requires `zenity` as well as `resolvconf` which will need to be installed.

In a terminal run the following.

```
sudo apt install zenity resolvconf
```

Download the latest deb package from https://github.com/jeremehancock/dnsminder/tree/main/deb.

In a terminal run the following from the directory where the deb package was downloaded.

```
sudo dpkg -i dnsminder_x.x.x_all.deb
```

Replace x.x.x with the latest version.

DNS Minder should now be available in your applications menu.

## How to use without installing:

DNS Minder requires `zenity` as well as `resolvconf` which will need to be installed and enabled.

In a terminal run the following.

```
sudo apt install zenity resolvconf
```

```
sudo systemctl enable --now resolvconf.service
```

```
git clone https://github.com/jeremehancock/dnsminder.git
```

```
cd dnsminder
```

```
./dnsminder.sh
```

## Disclaimer

All code is provided as-is without any warranty. This tool will download and setup a new hosts file. It will be making
changes to your system and should be USED AT YOUR OWN RISK!
