# Shell

## 查看 cronjob log

```sh
sudo tail -f /var/log/syslog | grep CRON
sudo journalctl -u cron.service -f
```

## description of system path

```bash
man hier
```

```
HIER(7)                                       Linux Programmer's Manual                                       HIER(7)

NAME
       hier - description of the filesystem hierarchy

DESCRIPTION
       A typical Linux system has, among others, the following directories:

       /      This is the root directory.  This is where the whole tree starts.

       /bin   This  directory contains executable programs which are needed in single user mode and to bring the sys‐
              tem up or repair it.

       /boot  Contains static files for the boot loader.  This directory holds only the files which are needed during
              the  boot process.  The map installer and configuration files should go to /sbin and /etc.  The operat‐
              ing system kernel (initrd for example) must be located in either / or /boot.

       /dev   Special or device files, which refer to physical devices.  See mknod(1).

       /etc   Contains configuration files which are local to the machine.  Some larger software packages, like  X11,
              can  have  their own subdirectories below /etc.  Site-wide configuration files may be placed here or in
              /usr/etc.  Nevertheless, programs should always look for these files in /etc and you may have links for
              these files to /usr/etc.
...
...
...
```
