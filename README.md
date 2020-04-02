# Base Files for Anonymity Distribution Workstations #

Contains a marker file /usr/share/anon-ws-base-files/workstation that allows
other applications to identify, that they are running inside an Anonymity
Distribution Workstation.

Whonix-Workstation grub branding, motd and issue banner.

Sets Xfce desktop and display setting, wallpaper and desktop icons.
/etc/skel/.config/xfce4/xfconf/xfce-perchannel-xml/xfce4-desktop.xml.anondist

Do not remove, unless you no longer wish to use an Anonymity Distribution
Workstation.
## How to install `anon-ws-base-files` using apt-get ##

1\. Download [Whonix's Signing Key]().

```
wget https://www.whonix.org/patrick.asc
```

Users can [check Whonix Signing Key](https://www.whonix.org/wiki/Whonix_Signing_Key) for better security.

2\. Add Whonix's signing key.

```
sudo apt-key --keyring /etc/apt/trusted.gpg.d/whonix.gpg add ~/patrick.asc
```

3\. Add Whonix's APT repository.

```
echo "deb https://deb.whonix.org buster main contrib non-free" | sudo tee /etc/apt/sources.list.d/whonix.list
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

See [instructions](https://www.whonix.org/wiki/Dev/Build_Documentation/anon-ws-base-files). (Replace `package-name` with the actual name of this package.)

## Contact ##

* [Free Forum Support](https://forums.whonix.org)
* [Professional Support](https://www.whonix.org/wiki/Professional_Support)

## Donate ##

`anon-ws-base-files` requires [donations](https://www.whonix.org/wiki/Donate) to stay alive!
