ets_fps_mmi-y += ets_fps.o
ets_fps_mmi-$(CONFIG_INPUT_EGISTEC_FPS_NAVI) += ets_navi_input.o

obj-$(CONFIG_FINGERPRINT_EGISTEC_FPS_MMI) += ets_fps_mmi.o

ifneq ($(filter doha%, $(TARGET_PRODUCT)),)
EXTRA_CFLAGS += -DCONFIG_INPUT_EGISTEC_FPS_POSE=0
else
EXTRA_CFLAGS += -DCONFIG_INPUT_EGISTEC_FPS_POSE=270
endif

ifneq ($(filter sofia%, $(TARGET_PRODUCT)),)
EXTRA_CFLAGS += -DCONFIG_INPUT_EGISTEC_FPS_POSE=0
endif
ifneq ($(filter rav%, $(TARGET_PRODUCT)),)
EXTRA_CFLAGS += -DCONFIG_INPUT_EGISTEC_FPS_POSE=0
endif
