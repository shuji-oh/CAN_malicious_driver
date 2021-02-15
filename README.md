# CAN_malicious_driver

## requirements
`linux-headers-$(uname -r)`  
or  
`raspberrypi-kernel-headers`  
if you use raspbery pi, you can build the kernel headers by following URL.  
https://github.com/RPi-Distro/rpi-source  

## mcp251x
This is the default spi driver for mcp2510, mcp2515.

### build/install
```
$ git clone https://github.com/shuji-oh/CAN_malicious_driver  
$ cd CAN_malicious_driver/mcp251x/  
$ make  
$ sudo insmod mcp251x.ko
```

## mcp251x_disabled_busoff
This is the spi driver which is disabled busoff state for mcp2510, mcp2515.

### build/install
```
$ git clone https://github.com/shuji-oh/CAN_malicious_driver  
$ cd CAN_malicious_driver/mcp251x_disabled_busoff/  
$ make  
$ sudo insmod mcp251x_disabled_busoff.ko
```

## mcp251x_kernel_sniffing
This is the spi driver to sniff the CAN messages on kernel land for mcp2510, mcp2515.

### build/install
```
$ git clone https://github.com/shuji-oh/CAN_malicious_driver  
$ cd CAN_malicious_driver/mcp251x_kernel_sniffing/  
$ make  
$ sudo insmod mcp251x_kernel_sniffing.ko
```
