ARG TAG=3.20.3
FROM alpine:${TAG}@sha256:33735bd63cf84d7e388d9f6d297d348c523c044410f553bd878c6d7829612735

RUN apk update

RUN apk add --no-cache dotnet8-sdk=8.0.111-r0 git=2.45.2-r0 bash

ENV DOTNET_RUNNING_IN_CONTAINER=true 
ENV DOTNET_USE_POLLING_FILE_WATCHER=true
ENV DOTNET_NOLOGO=true
ENV DOTNET_CLI_WORKLOAD_UPDATE_NOTIFY_DISABLE=true
ENV DOTNET_ROOT=/usr/bin/

# Change the default shell to bash
SHELL ["/bin/bash", "-c"]

CMD [ "/bin/bash" ]