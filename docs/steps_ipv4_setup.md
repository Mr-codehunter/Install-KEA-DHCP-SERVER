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

## Step 4

Now you can see three auto generated file through above command.

We will `move` the auto-generated configuration file in same location for future references.

```
mv /etc/kea/kea-dhcp4.conf /etc/kea/kea-dhcp4.conf.reference
```

## step 5

Now we are make new configuration file in same location `/etc/kea/`.

```
touch kea-dhcp4.conf
```

```
vim kea-dhcp4.conf
```
Configuration file is here :

# [conf file of ipv4](kea-dhcp4.conf)

Paste it on `kea-dhcp4.conf` file.

## Step 6

Create `kea-dhcp-ddns.conf` in `/etc/kea` directory.

```
touch kea-dhcp-ddns.conf
```

```
vim kea-dhcp-ddns.conf
```

`kea-dhcp-ddns.conf` file is here :

# [kea-dhcp-ddns.conf file](kea-dhcp-ddns.conf)
