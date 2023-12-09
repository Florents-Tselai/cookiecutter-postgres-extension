ARG PG_MAJOR={{ cookiecutter.pg_major_version}}
FROM postgres:$PG_MAJOR
ARG PG_MAJOR

COPY . /tmp/{{ cookiecutter.extension_name }}

RUN apt-get update && \
		apt-mark hold locales && \
		apt-get install -y --no-install-recommends build-essential postgresql-server-dev-$PG_MAJOR && \
		cd /tmp/{{ cookiecutter.extension_name }} && \
		make clean && \
		make OPTFLAGS="" && \
		make install && \
		mkdir /usr/share/doc/{{ cookiecutter.extension_name }} && \
		cp LICENSE README.md /usr/share/doc/{{ cookiecutter.extension_name }} && \
		rm -r /tmp/{{ cookiecutter.extension_name }} && \
		apt-get remove -y build-essential postgresql-server-dev-$PG_MAJOR && \
		apt-get autoremove -y && \
		apt-mark unhold locales && \
		rm -rf /var/lib/apt/lists/*
