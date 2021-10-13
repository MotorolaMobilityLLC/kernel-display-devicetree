ifneq ($(CONFIG_ARCH_QTI_VM), y)
#remove useless qcom device tree in moto build
ifneq ($(CONFIG_MMI_DEVICE_DTBS),y)
dtbo-y += display/waipio-sde.dtbo \
		display/waipio-sde-display-mtp-overlay.dtbo \
		display/waipio-sde-display-cphy-mtp-overlay.dtbo \
		display/waipio-sde-display-cdp-overlay.dtbo \
		display/waipio-sde-display-qrd-overlay.dtbo \
		display/waipio-sde-display-hdk-overlay.dtbo \
		display/waipio-sde-display-waipio-lemur-cdp-overlay.dtbo \
		display/waipio-sde-display-waipio-lemur-mtp-overlay.dtbo \
		display/waipio-sde-display-rumi-overlay.dtbo
else
# Li display bringup
ifeq ($(CONFIG_LI_DTB),y)
dtbo-y += display/waipio-sde.dtbo \
		display/waipio-sde-display-li-evb1-overlay.dtbo
else
dtbo-y += display/waipio-sde.dtbo \
		display/waipio-sde-display-hiphi-evb1-overlay.dtbo \
		display/waipio-sde-display-hiphic-evb1-overlay.dtbo\
		display/waipio-mot-ironmn-display-evb1-overlay.dtbo
endif  #($CONFIG_LI_DTB,y)
endif  #($(CONFIG_MMI_DEVICE_DTBS),y)
else
dtbo-y += display/trustedvm-waipio-sde-display-mtp-overlay.dtbo \
	  display/trustedvm-waipio-sde-display-cdp-overlay.dtbo \
	  display/trustedvm-waipio-sde-display-rumi-overlay.dtbo \
	  display/trustedvm-waipio-sde-display-qrd-overlay.dtbo
endif
always-y    := $(dtb-y) $(dtbo-y)
subdir-y    := $(dts-dirs)
clean-files    := *.dtb *.dtbo
