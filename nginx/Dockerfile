# https://hub.docker.com/_/nginx/
FROM arm64v8/nginx:1.17.6-alpine

COPY templates /opt/templates
COPY docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh
RUN chmod +x /usr/local/bin/docker-entrypoint.sh

ENTRYPOINT ["docker-entrypoint.sh"]
CMD ["-g", "daemon off;"]
