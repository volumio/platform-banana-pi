# platform-banana-pi

### Files for bananapi platform   

* kernel_3_4_113_w_olfs.tgz
* currently armhf build kernel with overlayFS support
and SPDIF support
* mainly adapted from bananian.org
* including boot partition files

## choose kernel options

in build/scripts/bpiproimage.sh you can choose which kernel you like by commenting option blocks in resp out

## load kernel modules

optional modules are

### powersave options

```
cpufreq_conservative
cpufreq_userspace 
cpufreq_stats 
cpufreq_powersave 
```

### spdif sound interface

```
sunxi_spdma
sunxi_spdif 
sunxi_sndspdif 
sndspdif 
```

### WLAN

```
ap6210 
```


insert module names in /etc/modules (one in each line)

