#
# Makefile for nfc devices
#

obj-$(CONFIG_NFC_PN544)		+= pn544/
obj-$(CONFIG_NFC_MICROREAD)	+= microread/
obj-$(CONFIG_NFC_PN533)		+= pn533.o
obj-$(CONFIG_NFC_WILINK)	+= nfcwilink.o
obj-$(CONFIG_NFC_MEI_PHY)	+= mei_phy.o
obj-$(CONFIG_NFC_SIM)		+= nfcsim.o
obj-$(CONFIG_NFC_PORT100)	+= port100.o
obj-$(CONFIG_NFC_MRVL)		+= nfcmrvl/
obj-$(CONFIG_NFC_TRF7970A)	+= trf7970a.o
obj-$(CONFIG_NFC_ST21NFCA)  	+= st21nfca/
obj-$(CONFIG_NFC_ST21NFCB)	+= st21nfcb/
ifdef CONFIG_VENDOR_SMARTISAN
obj-$(CONFIG_NFC_NQ)		+= nq-nci_smartisan.o
else
obj-$(CONFIG_NFC_NQ)		+= nq-nci.o
endif

ifdef CONFIG_VENDOR_SMARTISAN
obj-$(CONFIG_BCM2079X_NFC)	+= bcm2079x-i2c.o
obj-$(CONFIG_NXP_NFC_NQ220)	+= pn547.o
endif

ccflags-$(CONFIG_NFC_DEBUG) := -DDEBUG
