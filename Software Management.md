- yum/dnf
- rpm (RedHat Package Manager)

# yum/dnf
```bash
yum install httpd

```

```bash
root@rhcsa:~# yum list httpd
Updating Subscription Management repositories.
Red Hat Enterprise Linux 10 for x86_64 - AppStream (RPMs)                                  25 kB/s | 4.1 kB     00:00
Red Hat Enterprise Linux 10 for x86_64 - BaseOS (RPMs)                                      21 kB/s | 4.1 kB     00:00
Installed Packages
httpd.x86_64
```

```bash
root@rhcsa:/etc/yum.repos.d# yum repolist
Updating Subscription Management repositories.
repo id                                           repo name
rhel-10-for-x86_64-appstream-rpms                 Red Hat Enterprise Linux 10 for x86_64 - AppStream (RPMs)
rhel-10-for-x86_64-baseos-rpms                    Red Hat Enterprise Linux 10 for x86_64 - BaseOS (RPMs)
root@rhcsa:/etc/yum.repos.d#
```

# rpm
```bash
rpm -qa
rpm -qvp httpd

```

```bash
root@rhcsa:~# rpm -ql httpd
/etc/httpd/conf.modules.d/00-brotli.conf
/etc/httpd/conf.modules.d/00-systemd.conf
/usr/lib/.build-id
/usr/lib/.build-id/8a
/usr/lib/.build-id/8a/43e709dd411b1e4c05eab82b4dd10a8f5686bf
/usr/lib/.build-id/cc
/usr/lib/.build-id/cc/35b3caabc51c6734420fd912b64076337b75ca
/usr/lib/systemd/system/htcacheclean.service
/usr/lib/systemd/system/httpd.service
/usr/lib/systemd/system/httpd.socket
/usr/lib/systemd/system/httpd@.service
/usr/lib64/httpd/modules/mod_brotli.so
/usr/lib64/httpd/modules/mod_systemd.so
/usr/share/man/man5/httpd.conf.5.gz
/usr/share/man/man8/apachectl.8.gz
/usr/share/man/man8/fcgistarter.8.gz
/usr/share/man/man8/htcacheclean.8.gz
/usr/share/man/man8/htcacheclean.service.8.gz
/usr/share/man/man8/httpd.8.gz
/usr/share/man/man8/httpd.service.8.gz
/usr/share/man/man8/httpd.socket.8.gz
/usr/share/man/man8/httpd@.service.8.gz
/usr/share/man/man8/rotatelogs.8.gz
/usr/share/man/man8/suexec.8.gz
root@rhcsa:~#
```