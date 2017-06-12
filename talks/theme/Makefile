.PHONY: default css watch clean

input_dir := source
output_dir := css

sources := $(wildcard $(input_dir)/tuos-lib-*.scss)
compiled := $(sources:$(input_dir)/%.scss=$(output_dir)/%.css)
mappings := $(compiled:%=%.map)

default: css

css: $(compiled)

watch:
	sass --watch $(input_dir):$(output_dir)

clean:
	rm -f $(compiled)
	rm -f $(mappings)

$(output_dir)/%.css: $(input_dir)/%.scss $(input_dir)/_tuos-lib-base.scss
	sass $< $@
