ifeq ($(CONFIG_ARCH_KALAMA), y)
	dtbo-y += display/kalama-sde.dtbo \
		display/kalama-sde-display-rumi-overlay.dtbo
endif
ifeq ($(CONFIG_ARCH_WAIPIO), y)
        dtbo-y += display/waipio-sde.dtbo \
                  display/waipio-sde-display-mtp-overlay.dtbo \
                  display/waipio-sde-display-cphy-mtp-overlay.dtbo \
                  display/waipio-sde-display-cdp-overlay.dtbo \
                  display/waipio-sde-display-qrd-overlay.dtbo \
                  display/waipio-sde-display-hdk-overlay.dtbo \
                  display/waipio-sde-display-waipio-lemur-cdp-overlay.dtbo \
                  display/waipio-sde-display-waipio-lemur-mtp-overlay.dtbo \
                  display/waipio-sde-display-rumi-overlay.dtbo

endif
always-y    := $(dtb-y) $(dtbo-y)
subdir-y    := $(dts-dirs)
clean-files    := *.dtb *.dtbo
