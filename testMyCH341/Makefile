#在虚拟机平台linux 运行hello
#https://note.youdao.com/ynoteshare1/index.html?id=76ee5277efcab20451f220ba3e792e16&type=note

KERN_DIR = /lib/modules/$(shell uname -r)/build
 
all:
	make -C $(KERN_DIR) M=`pwd` modules
 
clean:
	make -C $(KERN_DIR) M=$(shell pwd) modules clean
	rm -rf modules.order
 
obj-m := myCh341.o
