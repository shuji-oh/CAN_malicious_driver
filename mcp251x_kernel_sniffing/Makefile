
KERNEL_DIR = /lib/modules/$(shell uname -r)/build

obj-m := mcp251x_kernel_sniffing.o

all:
	make -C $(KERNEL_DIR) M=$(shell pwd) modules
clean:
	make -C $(KERNEL_DIR) M=$(shell pwd) clean
