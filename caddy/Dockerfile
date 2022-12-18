#FROM caddy:2.5.1-builder AS builder
#RUN xcaddy build \
#    --with github.com/miekg/caddy-prometheus \
#    --with github.com/pyed/ipfilter@v1.1.4

FROM caddy:2.5.1
#COPY --from=builder /usr/bin/caddy /usr/bin/caddy
COPY Caddyfile /etc/caddy/Caddyfile
RUN apk add curl nss-tools
