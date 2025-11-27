FROM gcr.io/distroless/static:latest

ARG TARGETOS TARGETARCH
# RUN echo $TARGETOS
# RUN echo $TARGETARCH

COPY build/$TARGETOS-$TARGETARCH/oneclick-mesh-client /oneclick-mesh-client
COPY build/$TARGETOS-$TARGETARCH/oneclick-mesh-client-cert /oneclick-mesh-client-cert

VOLUME ["/config"]

ENTRYPOINT ["/oneclick-mesh-client"]
# Allow users to override the args passed to nebula
CMD ["-config", "/config/config.yml"]
