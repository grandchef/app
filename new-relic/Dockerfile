FROM base

RUN apk add gcompat

# Install new relic agent
RUN \
  curl -L https://download.newrelic.com/php_agent/release/newrelic-php5-10.7.0.319-linux-musl.tar.gz | tar -C /tmp -zx && \
  export NR_INSTALL_USE_CP_NOT_LN=1 && \
  export NR_INSTALL_SILENT=1 && \
  /tmp/newrelic-php5-*/newrelic-install install && \
  rm -rf /tmp/newrelic-php5-* /tmp/nrinstall
