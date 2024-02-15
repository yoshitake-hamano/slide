# File: Makefile - last edit
# yoshitake 16-Feb-2024

SRC_DIR:=src
BUILD_DIR:=images
SOURCES:=$(wildcard $(SRC_DIR)/*.puml)
TARGETS:=$(addprefix $(BUILD_DIR)/,$(notdir $(SOURCES:.puml=.png)))

all: $(TARGETS)

.PHONY: clean
clean:
	$(RM) $(TARGETS)

$(BUILD_DIR)/%.png: $(SRC_DIR)/%.puml
	plantuml -Tpng -o ../$(BUILD_DIR) $^

# Log
# 16-Feb-2024 yoshitake Created.
