PG_CONFIG ?= pg_config

EXTENSION = {{cookiecutter.extension_name}}
EXTVERSION = {{cookiecutter.default_version}}


MODULE_big = $(EXTENSION)
DATA = $(wildcard sql/*--*.sql)
SRCS = src/{{cookiecutter.extension_name}}.c
OBJS = src/{{cookiecutter.extension_name}}.o
HEADERS = src/$(EXTENSION).h

HEADERS_{{cookiecutter.extension_name}} = src/$(EXTENSION).h

TESTS = $(wildcard test/sql/*.sql)
REGRESS = $(patsubst test/sql/%.sql,%,$(TESTS))
REGRESS_OPTS = --inputdir=test --load-extension=$(EXTENSION)

PGXS := $(shell $(PG_CONFIG) --pgxs)
include $(PGXS)
