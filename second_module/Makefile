obj-m += deadlock.o
module_name=deadlock.ko

all:
	make -C /lib/modules/$(shell uname -r)/build M=$(PWD) modules
	sudo insmod $(module_name)

clean:
	make -C /lib/modules/$(shell uname -r)/build M=$(PWD) clean
	sudo rmmod $(module_name)
