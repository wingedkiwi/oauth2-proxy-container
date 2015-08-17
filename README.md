# OAuth2 Proxy Container
_OAuth2 Proxy Container_ is a Docker Image of [_oauth2_proxy_](https://github.com/bitly/oauth2_proxy). An _Automated Build_ is setup at https://hub.docker.com/r/wingedkiwi/oauth2_proxy/.

## Run
    # Using a premounted configuration file in /opt/oauth2_proxy/etc/config
    docker run --rm -it wingedkiwi/oauth2_proxy

    # Using command line flags
    docker run --rm -it wingedkiwi/oauth2_proxy oauth2_proxy \
      --email-domain="yourcompany.com" \
      --upstream=http://127.0.0.1:8080/ \
      --cookie-secret=... \
      --client-id=... \
      --client-secret=...


