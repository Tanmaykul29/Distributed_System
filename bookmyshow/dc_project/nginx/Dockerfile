FROM nginx:1.19.0

COPY ./nginx/default.conf /etc/nginx/conf.d/nginx.conf

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]