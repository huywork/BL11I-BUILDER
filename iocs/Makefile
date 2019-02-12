TOP = ..
include $(TOP)/configure/CONFIG
DIRS := $(DIRS) $(filter-out Makefile, $(wildcard *))
include $(TOP)/configure/RULES_DIRS

# re-enable below instead of above for mixed architecture
# with specific ioc names

#TOP = ..
#include $(TOP)/configure/CONFIG
#
#ifeq ($(EPICS_HOST_ARCH), linux-x86)
#	DIRS := $(wildcard example example_sim)
#else ifeq ($(EPICS_HOST_ARCH), linux-x86_64)
#	DIRS :=
#else ifeq ($(EPICS_HOST_ARCH), win32-x86)
#	DIRS :=
#endif

#include $(TOP)/configure/RULES_DIRS
