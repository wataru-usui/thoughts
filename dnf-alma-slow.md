dnf make-cache was insanely slow at a few KB/s on almalinux 9.4 on laptop.
adding this to /etc/dnf/dnf.conf solved it and it went to a few MB/s

```
fastestmirror=True
max_parallel_downloads=10
```
