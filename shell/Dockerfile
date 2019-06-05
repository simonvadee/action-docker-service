FROM debian:stable-slim

LABEL "name"="shell"
LABEL "maintainer"="Simon Vadée <simon.vadee@gmail.com>"
LABEL "version"="0.0.1"

LABEL "com.github.actions.name"="Run shell commands"
LABEL "com.github.actions.icon"="terminal"
LABEL "com.github.actions.color"="gray-dark"

RUN apt-get update && apt-get install -y \
    openssh-client && \
    rm -Rf /var/lib/apt/lists/*

COPY entrypoint.sh /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]