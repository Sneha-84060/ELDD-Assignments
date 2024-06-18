
obj-m = pchar.o

modules:
	make ARCH=arm CROSS_COMPILE=arm-linux-gnueabihf- -C /home/user/linux/ M=`pwd` modules
	#make -C /lib/modules/`uname -r`/build M=`pwd` modules
copy:
	scp pchar.ko debian@192.168.7.2:/home/debian/Sneha
clean:
	make ARCH=arm CROSS_COMPILE=arm-linux-gnueabihf- -C /home/user/linux/ M=`pwd` clean

.phony: modules clean
