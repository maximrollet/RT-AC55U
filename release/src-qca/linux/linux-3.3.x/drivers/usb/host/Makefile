#
# Makefile for USB Host Controller Drivers
#

ccflags-$(CONFIG_USB_DEBUG) := -DDEBUG

isp1760-y := isp1760-hcd.o isp1760-if.o

fhci-y := fhci-hcd.o fhci-hub.o fhci-q.o
fhci-y += fhci-mem.o fhci-tds.o fhci-sched.o

fhci-$(CONFIG_FHCI_DEBUG) += fhci-dbg.o

obj-$(CONFIG_USB_XHCI_HCD)	+= etxhci-hcd.o
etxhci-hcd-objs := .objs/xhci-dbg.o .objs/xhci-ejxxx.o .objs/xhci-hub.o .objs/xhci-mem.o .objs/xhci.o .objs/xhci-pci.o .objs/xhci-ring.o

obj-$(CONFIG_USB_WHCI_HCD)	+= whci/

obj-$(CONFIG_PCI)		+= pci-quirks.o

obj-$(CONFIG_USB_EHCI_HCD)	+= ehci-hcd.o
obj-$(CONFIG_USB_OXU210HP_HCD)	+= oxu210hp-hcd.o
obj-$(CONFIG_USB_ISP116X_HCD)	+= isp116x-hcd.o
obj-$(CONFIG_USB_ISP1362_HCD)	+= isp1362-hcd.o
obj-$(CONFIG_USB_OHCI_HCD)	+= ohci-hcd.o
obj-$(CONFIG_USB_UHCI_HCD)	+= uhci-hcd.o
obj-$(CONFIG_USB_FHCI_HCD)	+= fhci.o
obj-$(CONFIG_USB_SL811_HCD)	+= sl811-hcd.o
obj-$(CONFIG_USB_SL811_CS)	+= sl811_cs.o
obj-$(CONFIG_USB_U132_HCD)	+= u132-hcd.o
obj-$(CONFIG_USB_R8A66597_HCD)	+= r8a66597-hcd.o
obj-$(CONFIG_USB_ISP1760_HCD)	+= isp1760.o
obj-$(CONFIG_USB_HWA_HCD)	+= hwa-hc.o
obj-$(CONFIG_USB_IMX21_HCD)	+= imx21-hcd.o
obj-$(CONFIG_USB_FSL_MPH_DR_OF)	+= fsl-mph-dr-of.o
obj-$(CONFIG_USB_OCTEON2_COMMON) += octeon2-common.o
obj-$(CONFIG_MIPS_ALCHEMY)	+= alchemy-common.o
