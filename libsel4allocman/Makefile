#
# Copyright 2017, Data61
# Commonwealth Scientific and Industrial Research Organisation (CSIRO)
# ABN 41 687 119 230.
#
# This software may be distributed and modified according to the terms of
# the BSD 2-Clause license. Note that NO WARRANTY is provided.
# See "LICENSE_BSD2.txt" for details.
#
# @TAG(DATA61_BSD)
#

# Targets
TARGETS := libsel4allocman.a

# Source files required to build the target
CFILES := $(sort $(patsubst $(SOURCE_DIR)/%,%,$(wildcard $(SOURCE_DIR)/src/*.c)))
CFILES += $(sort $(patsubst $(SOURCE_DIR)/%,%,$(wildcard $(SOURCE_DIR)/src/cspace/*.c)))
CFILES += $(sort $(patsubst $(SOURCE_DIR)/%,%,$(wildcard $(SOURCE_DIR)/src/utspace/*.c)))
CFILES += $(sort $(patsubst $(SOURCE_DIR)/%,%,$(wildcard $(SOURCE_DIR)/src/mspace/*.c)))

# Header files/directories this library provides
HDRFILES := $(sort $(wildcard $(SOURCE_DIR)/include/*)) \
    $(sort $(wildcard ${SOURCE_DIR}/sel4_arch/${SEL4_ARCH}/*))

CFLAGS += -std=gnu99

include $(SEL4_COMMON)/common.mk
