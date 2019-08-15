# squashfs-init

A wrapper script for the sqaushfs with interactive and init support

(C) Pavel Andreev (pasha132 at gmail.com).
The license of this package is the BSD 2-Clause “Simplified” License.

This package provides a module to manage and configure sqaushfs images
via individual per-image scripts in /etc/init.d.

Provided is the parent script "/etc/init.d/squashfs", which should be symlinked to
create additional scripts for each image to be configured:
```bash
        ln -s /etc/init.d/sqaushfs{,fs}
```

Configuration is handled in "/etc/conf.d/squashfs".  

To use compression with squashfs your kernel and squashfs-tools needs to be compiled with
a corresponding options. 
