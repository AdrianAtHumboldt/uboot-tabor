X86DIR  = x86emu

$(shell mkdir -p $(obj)$(X86DIR))

obj-y	= atibios.o biosemu.o besys.o bios.o vesa.o \
	$(X86DIR)/decode.o \
	$(X86DIR)/ops2.o \
	$(X86DIR)/ops.o \
	$(X86DIR)/prim_ops.o \
	$(X86DIR)/sys.o \
	$(X86DIR)/debug.o

ccflags-y := -I$(srctree)/$(src) -I$(srctree)/$(src)/include \
	-D__PPC__  -D__BIG_ENDIAN__
