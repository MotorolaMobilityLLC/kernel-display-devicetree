ifneq ($(CONFIG_ARCH_QTI_VM), y)
dtbo-$(CONFIG_ARCH_KALAMA) += display/kalama-sde.dtbo \
		display/kalama-sde-display-rumi-overlay.dtbo \
		display/kalama-sde-display-cdp-overlay.dtbo \
		display/kalama-sde-display-cdp-wsa883x-overlay.dtbo \
		display/kalama-sde-display-mtp-overlay.dtbo \
		display/kalama-sde-display-qrd-overlay.dtbo \
		display/kalama-sde-display-hdk-overlay.dtbo \
		display/kalama-sde-display-hhg-overlay.dtbo \
		display/kalama-sde-display-mtp-nfc-overlay.dtbo \
		display/kalama-sde-display-rcm-overlay.dtbo \
		display/kalama-sde-display-cdp-nfc-overlay.dtbo \
		display/kalama-sde-display-atp-overlay.dtbo
else
dtbo-$(CONFIG_ARCH_KALAMA) += display/trustedvm-kalama-sde-display-mtp-overlay.dtbo \
                  display/trustedvm-kalama-sde-display-mtp-nfc-overlay.dtbo \
                  display/trustedvm-kalama-sde-display-cdp-nfc-overlay.dtbo \
		  display/trustedvm-kalama-sde-display-cdp-overlay.dtbo \
		  display/trustedvm-kalama-sde-display-cdp-wsa883x-overlay.dtbo \
		  display/trustedvm-kalama-sde-display-rumi-overlay.dtbo \
		  display/trustedvm-kalama-sde-display-qrd-overlay.dtbo \
		  display/trustedvm-kalama-sde-display-atp-overlay.dtbo
endif

ifneq ($(CONFIG_ARCH_QTI_VM), y)
dtbo-$(CONFIG_ARCH_CROW) += display/crow-sde.dtbo \
		display/crow-sde-display-idp-overlay.dtbo \
		display/crow-sde-display-idp-wcd-overlay.dtbo \
		display/crow-sde-display-atp-overlay.dtbo \
		display/crow-sde-display-rumi-overlay.dtbo \
		display/crow-sde-display-qrd-overlay.dtbo \
		display/crow-sde-display-idps-overlay.dtbo \
		display/crow-sde-display-idps-wcd-overlay.dtbo
else
dtbo-$(CONFIG_ARCH_CROW) += display/trustedvm-crow-sde-display-idp-overlay.dtbo \
		  display/trustedvm-crow-sde-display-idp-wcd-overlay.dtbo \
		  display/trustedvm-crow-sde-display-atp-overlay.dtbo \
		  display/trustedvm-crow-sde-display-rumi-overlay.dtbo \
		  display/trustedvm-crow-sde-display-qrd-overlay.dtbo
endif

ifeq ($(CONFIG_ARCH_SA8155), y)
dtbo-y += display/sa8155-adp-star-display.dtbo
endif

ifneq ($(CONFIG_ARCH_QTI_VM), y)
dtbo-$(CONFIG_ARCH_WAIPIO) += display/waipio-sde.dtbo \
		display/waipio-sde-display-mtp-overlay.dtbo \
		display/waipio-sde-display-cphy-mtp-overlay.dtbo \
		display/waipio-sde-display-cdp-overlay.dtbo \
		display/waipio-sde-display-qrd-overlay.dtbo \
		display/waipio-sde-display-hdk-overlay.dtbo \
		display/waipio-sde-display-waipio-lemur-cdp-overlay.dtbo \
		display/waipio-sde-display-waipio-lemur-mtp-overlay.dtbo \
		display/waipio-sde-display-rumi-overlay.dtbo
else
dtbo-$(CONFIG_ARCH_WAIPIO) += display/trustedvm-waipio-sde-display-mtp-overlay.dtbo \
		display/trustedvm-waipio-sde-display-cdp-overlay.dtbo \
		display/trustedvm-waipio-sde-display-rumi-overlay.dtbo \
		display/trustedvm-waipio-sde-display-qrd-overlay.dtbo
endif

always-y    := $(dtb-y) $(dtbo-y)
subdir-y    := $(dts-dirs)
clean-files    := *.dtb *.dtbo
