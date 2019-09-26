# Graph 
## A lean desktop environment over RDP protocol using CentOS + GNOME + XRDP

This is an example of how an environmentally friendly desktop environment can be simply configured for various applications to suit each individual's needs.


First we need to install GNOME desktop

```
yum -y groups install "GNOME Desktop"
```


Add XRDP source
```
rpm -Uvh https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm
```

Now we need to install XRDP to connect through RDP protocol
```
yum -y install xrdp tigervnc-server
```

Start service and enable for autostart on boot
```
systemctl start xrdp
systemctl enable xrdp
```
