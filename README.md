# Base Files for Anonymity Distribution Workstations #

Contains a marker file /usr/share/anon-ws-base-files/workstation that allows
other applications to identify, that they are running inside an Anonymity
Distribution Workstation.

Whonix-Workstation grub branding, motd and issue banner.

Sets Xfce desktop and display setting, wallpaper and desktop icons.
/etc/skel/.config/xfce4/xfconf/xfce-perchannel-xml/xfce4-desktop.xml.anondist

Extra Start Menu Entries for Whonix-Workstation
Contains start menu entries for the following links:
- contribute
- donate
- forum
- mailinglist
- documentation
- featureblog
- importantblog

Do not remove, unless you no longer wish to use an Anonymity Distribution
Workstation.

## How to install `anon-ws-base-files` using apt-get ##

1\. Download the APT Signing Key.

```
wget https://www.whonix.org/keys/derivative.asc
```

Users can [check the Signing Key](https://www.whonix.org/wiki/Signing_Key) for better security.

2\. Add the APT Signing Key.

```
sudo cp ~/derivative.asc /usr/share/keyrings/derivative.asc
```

3\. Add the derivative repository.

```
echo "deb [signed-by=/usr/share/keyrings/derivative.asc] https://deb.whonix.org bookworm main contrib non-free" | sudo tee /etc/apt/sources.list.d/derivative.list
```

4\. Update your package lists.

```
sudo apt-get update
```

5\. Install `anon-ws-base-files`.

```
sudo apt-get install anon-ws-base-files
```

## How to Build deb Package from Source Code ##

Can be build using standard Debian package build tools such as:

```
dpkg-buildpackage -b
```

See instructions.

NOTE: Replace `generic-package` with the actual name of this package `anon-ws-base-files`.

* **A)** [easy](https://www.whonix.org/wiki/Dev/Build_Documentation/generic-package/easy), _OR_
* **B)** [including verifying software signatures](https://www.whonix.org/wiki/Dev/Build_Documentation/generic-package)

## Contact ##

* [Free Forum Support](https://forums.whonix.org)
* [Premium Support](https://www.whonix.org/wiki/Premium_Support)

## Donate ##

`anon-ws-base-files` requires [donations](https://www.whonix.org/wiki/Donate) to stay alive!
