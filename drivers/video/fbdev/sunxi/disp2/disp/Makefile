include $(obj)/de/Makefile

# define_trace.h needs to know how to find our header
CFLAGS_disp_trace.o := -I$(src)

obj-$(CONFIG_DISP2_SUNXI) += disp.o

disp-objs :=  dev_disp.o dev_fb.o dev_disp_debugfs.o
disp-objs += disp_sys_intf.o
disp-objs += disp_trace.o
disp-$(CONFIG_DISP2_SUNXI_COMPOSER) += dev_composer.o
disp-objs += de/disp_display.o de/disp_features.o de/disp_device.o \
	     de/disp_manager.o de/disp_private.o \
	     de/disp_smart_backlight.o de/disp_enhance.o de/disp_capture.o \
	     de/disp_hdmi.o de/disp_tv.o de/disp_vdevice.o \
	     de/disp_vga.o \
	     de/disp_vdpo.o de/disp_edp.o de/disp_rtwb.o
disp-$(CONFIG_EINK_PANEL_USED) += de/disp_eink_manager.o \
		de/eink_buffer_manager.o de/eink_pipeline_manager.o \
		de/disp_format_convert.o

disp-objs += de/disp_vga.o \
	     de/disp_vdpo.o de/disp_edp.o
disp-$(CONFIG_SUNXI_DISP2_FB_ROTATION_SUPPORT) += de/disp_rotation_sw.o
disp-$(CONFIG_SUNXI_DISP2_FB_HW_ROTATION_SUPPORT) += fb_g2d_rot.o

disp-objs += $(obj_low)
