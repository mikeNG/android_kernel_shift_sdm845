# SPDX-License-Identifier: GPL-2.0
ifneq ($(CONFIG_ARCH_SDM845),y)
dtb-$(CONFIG_ARCH_QCOM)	+= apq8016-sbc.dtb
dtb-$(CONFIG_ARCH_QCOM)	+= apq8096-db820c.dtb
dtb-$(CONFIG_ARCH_QCOM)	+= ipq8074-hk01.dtb
dtb-$(CONFIG_ARCH_QCOM)	+= msm8916-mtp.dtb
dtb-$(CONFIG_ARCH_QCOM)	+= msm8992-bullhead-rev-101.dtb
dtb-$(CONFIG_ARCH_QCOM)	+= msm8994-angler-rev-101.dtb
dtb-$(CONFIG_ARCH_QCOM)	+= msm8996-mtp.dtb
endif

ifeq ($(CONFIG_BUILD_ARM64_DT_OVERLAY),y)
dtbo-$(CONFIG_ARCH_QCOM) += \
	sdm845-mtp-overlay.dtbo \
	sdm845-qrd-overlay.dtbo \
	sdm845-v2-mtp-overlay.dtbo \
	sdm845-v2-qrd-overlay.dtbo \
	sdm845-v2.1-mtp-overlay.dtbo \
	sdm845-v2.1-qrd-overlay.dtbo

sdm845-mtp-overlay.dtbo-base := sdm845.dtb
sdm845-qrd-overlay.dtbo-base := sdm845.dtb
sdm845-v2-mtp-overlay.dtbo-base := sdm845-v2.dtb
sdm845-v2-qrd-overlay.dtbo-base := sdm845-v2.dtb
sdm845-v2.1-mtp-overlay.dtbo-base := sdm845-v2.1.dtb
sdm845-v2.1-qrd-overlay.dtbo-base := sdm845-v2.1.dtb
else
dtb-$(CONFIG_ARCH_QCOM)	+= sdm845-mtp.dtb
dtb-$(CONFIG_ARCH_QCOM)	+= sdm845-qrd.dtb
dtb-$(CONFIG_ARCH_QCOM)	+= sdm845-v2-mtp.dtb
dtb-$(CONFIG_ARCH_QCOM)	+= sdm845-v2-qrd.dtb
dtb-$(CONFIG_ARCH_QCOM)	+= sdm845-v2.1-mtp.dtb
endif

always		:= $(dtb-y)
subdir-y	:= $(dts-dirs)
clean-files    := *.dtb *.dtbo
