#-- Build CPU test program and create VHDL package with object code ------------

# All we do here is configure the build:

# Test name (same as dir name).
TEST = cpu_test
# Root file name of the only source file in this test.
SRCFILE = tb51_cpu
# XROM size in bytes. The CPU tester needs a bit more than 33K ox XCODE.
XCODE_SIZE = 40000
# XRAM size in bytes -- the minimum of 512 bytes will do.
XDATA_SIZE = 512

ifeq ($(BCD),1)
	BCD_FLAG = --define=BCD
else
	BCD =
endif

# The actual build happens in the main makefile fragment.
include ../include/assembler.mk
