
CURR_DIR=$(shell realpath .)
WASM_CLANG=/opt/wasi-sdk/bin/clang

build: $(CURR_DIR)/../echo_server$(WASM_OUT_SUFFIX).wasm

$(CURR_DIR)/../echo_server$(WASM_OUT_SUFFIX).wasm: main.cpp
	$(WASM_CLANG)++ $(WASM_CFLAGS) $< -o $@