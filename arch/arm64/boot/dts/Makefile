dtb-$(CONFIG_ARCH_VEXPRESS) += rtsm_ve-aemv8a.dtb foundation-v8.dtb \
				fvp-base-gicv2-psci.dtb
dtb-$(CONFIG_ARCH_VEXPRESS) += juno.dtb
dtb-$(CONFIG_ARCH_XGENE) += apm-mustang.dtb
dtb-$(CONFIG_MACH_ESPRESSO7420) += exynos7420-espresso7420.dtb exynos7420-universal7420-ufs.dtb
<<<<<<< HEAD
=======
dtb-$(CONFIG_G_NINE) += exynos7420-zeroflte_eur_open_06.dtb \
				    exynos7420-zeroflte_usa_05.dtb \
				    exynos7420-zeroflte_usa_cdma_03.dtb

dtb-$(CONFIG_G_NINE_F) += exynos7420-zerolte_eur_open_08.dtb \
				    exynos7420-zerolte_usa_06.dtb \
				    exynos7420-zerolte_usa_cdma_03.dtb

>>>>>>> d8cece8... Add Device tree build option for 920 / 925 and aif_checking in custom options

targets += dtbs

DTB_NAMES := $(subst $\",,$(CONFIG_BUILD_ARM64_APPENDED_DTB_IMAGE_NAMES))
ifneq ($(DTB_NAMES),)
DTB_LIST := $(addsuffix .dtb,$(DTB_NAMES))
else
DTB_LIST := $(dtb-y)
endif
targets += $(DTB_LIST)

dtbs: $(addprefix $(obj)/, $(DTB_LIST))

clean-files := dts/*.dtb *.dtb
