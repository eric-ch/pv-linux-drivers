ifneq ($(KERNELRELEASE),)
# kbuild part of makefile
include Kbuild

else
# normal makefile
KERNEL_VERSION ?= `uname -r`
KERNEL_SRC ?= /lib/modules/$(KERNEL_VERSION)/build

default:
	$(MAKE) -C $(KERNEL_SRC) M=$$PWD

clean:
	$(MAKE) -C $(KERNEL_SRC) M=$$PWD clean

endif
