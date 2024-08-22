FROM nginx:1.10

RUN if [ -z "$(getent group lazy)" ]; then groupadd -g 1133 lazy; fi && \
    if [ -z "$(id -u lazy >/dev/null 2>&1; echo $?)" ]; then useradd -g lazy -u 1133 lazy; fi