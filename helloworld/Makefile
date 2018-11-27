ifeq ($(THEOS),)
  $(error THEOS is not set)
endif

export PATH := $(THEOS):$(PATH)
SHELL = /bin/bash

ARCHS = arm64
TARGET = iphone:clang::10.0

include $(THEOS)/makefiles/common.mk

TOOL_NAME = helloworld

helloworld_FILES = main.c
helloworld_CFLAGS =
helloworld_LDFLAGS =

include $(THEOS)/makefiles/tool.mk
