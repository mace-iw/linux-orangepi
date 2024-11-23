MIPI_DSI_IP_VERSION ?= 40

ifeq ($(CONFIG_ARCH_SUN50IW5T),y)
sub_dir = lowlevel_v33x
MIPI_DSI_IP_VERSION := 28
endif

ifeq ($(CONFIG_ARCH_SUN50IW9),y)
sub_dir = lowlevel_v33x
MIPI_DSI_IP_VERSION := 28
endif

ifeq ($(CONFIG_ARCH_SUN50IW5T),y)
sub_dir = lowlevel_v33x
MIPI_DSI_IP_VERSION := 28
endif

ifeq ($(CONFIG_ARCH_SUN50IW9),y)
sub_dir = lowlevel_v33x
MIPI_DSI_IP_VERSION := 28
endif

ifneq ($(sub_dir),)
-include $(obj)/de/$(sub_dir)/Makefile
endif
