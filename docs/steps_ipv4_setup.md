# Installation and configurations steps for ipv4 :

If you are not a root user/super user use `sudo` in the starting of any command.

Like : `sudo apt install <package_name>`

## Step 1 

- Install kea-server 

# [Installation](installation.md)

<p align="center">
  <img src="images/kea1.png" />
</p>

## Step 2

- Check status of kea-server

```
systemctl status kea-dhcp4-server
```

<p align="center">
  <img src="images/kea2.png" />
</p>

## Step 3

In this step root access is necessary.

Now go to `/etc/kea/` directory.

```
ls /etc/kea/
```
<p align="center">
  <img src="images/kea3.png" />
</p>

