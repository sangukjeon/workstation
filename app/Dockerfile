FROM nginx:alpine
LABEL org.opencontainers.image.title="my-workstation-web"
ENV APP_ENV=dev
COPY site/ /usr/share/nginx/html/
EXPOSE 80
HEALTHCHECK CMD wget -qO- http://localhost/ || exit 1