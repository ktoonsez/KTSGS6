ccflags-y := -Ofast -ffast-math -fgcse-lm -fgcse-sm -fsched-spec-load -fforce-addr -fsingle-precision-constant
obj-y				:= dma-mapping.o extable.o fault.o init.o \
				   cache.o copypage.o flush.o \
				   ioremap.o iomap.o mmap.o pgd.o mmu.o \
				   context.o tlb.o proc.o
obj-$(CONFIG_HUGETLB_PAGE)	+= hugetlbpage.o
