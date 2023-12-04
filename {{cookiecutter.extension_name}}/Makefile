PG_CONFIG ?= pg_config

EXTENSION = {{cookiecutter.extension_name}}
EXTVERSION = {{cookiecutter.default_version}}


MODULE_big = $(EXTENSION)
DATA = $(wildcard sql/*--*.sql)
SRCS = src/{{cookiecutter.extension_name}}.c
OBJS = src/{{cookiecutter.extension_name}}.o
HEADERS = src/$(EXTENSION).h

TESTS = $(wildcard test/sql/*.sql)
REGRESS = $(patsubst test/sql/%.sql,%,$(TESTS))
REGRESS_OPTS = --inputdir=test --load-extension=$(EXTENSION)

.PHONY: dist

dist:
	mkdir -p dist
	git archive --format zip --prefix=$(EXTENSION)-$(EXTVERSION)/ --output dist/$(EXTENSION)-$(EXTVERSION).zip main

PGXS := $(shell $(PG_CONFIG) --pgxs)
include $(PGXS)

