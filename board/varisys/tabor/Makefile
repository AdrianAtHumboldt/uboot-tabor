#
# Copyright 2010 Freescale Semiconductor, Inc.
#
# SPDX-License-Identifier:	GPL-2.0+
#

MINIMAL=

ifdef CONFIG_SPL_BUILD
ifdef CONFIG_SPL_INIT_MINIMAL
MINIMAL=y
endif
endif

ifdef MINIMAL

obj-y        += spl_minimal.o tlb.o law.o clk.o

else
ifdef CONFIG_SPL_BUILD
obj-y += spl.o
endif
obj-y	+= tabor.o
obj-y	+= ddr.o
obj-y	+= law.o
obj-y	+= tlb.o
obj-y   += clk.o

obj-$(CONFIG_FSL_DIU_FB) += diu.o
endif
