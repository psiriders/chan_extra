chan_extra
==========

Updated version of chan_extra driver for OpenVox G400P/G400E for kernel 3.10+ and Asterisk 11

#Installation instructions

After downloading the latest version of dahdi and uncompressing it, you will need to create a `.version` file in DAHDI directory that contains the current version number in order for the installation script to run properly.

**Example:**

```bash
cd /usr/src/dahdi-linux-complete-2.9.2+2.9.2
echo "2.9.2" > .version
```

After that, follow the official installation instructions for source install.

#Notes / Known issues

On latest Debian the `install.sh` script kept warning me about missing `bison-devel` package. You will have to install the package `libbison-dev` using the package manager yourself. The warning can be safely ignored after that.

**WARNING:** chan_extra fails to compile with DAHDI 2.10. For now, use 2.9.2 if you can. Once I get around to fixing this I will update the README with any additional info.
