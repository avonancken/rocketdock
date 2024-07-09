base_dir=$(abspath ./)

CHISEL_VERSION=3.6.0
MODEL ?=  MyAXISubsystem
PROJECT ?= tssv.componentgen
CFG_PROJECT ?= $(PROJECT)
CONFIG ?= $(CFG_PROJECT).MyAXIConfig
MILL ?= mill

verilog:
	cd $(base_dir) && $(MILL) emulator[$(PROJECT).$(MODEL),$(CONFIG)].mfccompiler.compile

clean:
	rm -rf out/
