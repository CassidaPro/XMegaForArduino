# Makefile for atxmega32e5 - invokes 'universal' Makefile in ../xmega
#
#

USE_TARGET=C400USB_Controller
CPU_TARGET=atxmega32e5


xmega:
	$(MAKE) -f Makefile.xmega xmega TARGET=$(USE_TARGET)A
	$(MAKE) -f Makefile.xmega xmega TARGET=$(USE_TARGET)B
	$(MAKE) -f Makefile.xmega xmega TARGET=$(USE_TARGET)C

#flashboot:
#	$(MAKE) -f Makefile.xmega fusesxmega TARGET=$(USE_TARGET)
#	avrdude -C avrdude.conf -c avrispmkii -p $(CPU_TARGET) -P usb -Uboot:w:xmegaBOOT_xmega0_$(USE_TARGET).hex:i -Ulockbits:w:0xBF:m

clean:
	$(MAKE) -f Makefile.xmega clean_$(USE_TARGET)A TARGET=$(USE_TARGET)A
	$(MAKE) -f Makefile.xmega clean_$(USE_TARGET)B TARGET=$(USE_TARGET)B
	$(MAKE) -f Makefile.xmega clean_$(USE_TARGET)C TARGET=$(USE_TARGET)C


