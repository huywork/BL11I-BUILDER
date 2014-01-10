TOP = ..
include $(TOP)/configure/CONFIG

ifeq (,$(findstring prod, $(shell pwd)))
  # If prod is not in pwd then make all the iocs
  DIRS := $(DIRS) $(filter-out $(wildcard Makefile*), $(wildcard *))
else
  # Otherwise just make simulations
  DIRS := $(DIRS) $(filter-out $(wildcard Makefile*), $(wildcard *_sim))
endif

include $(TOP)/configure/RULES_DIRS
