FROM wordpress:4.9.7-php7.2-apache
LABEL maintener Virgil de Lacerda <admin@virgapps.net>

ENV WORDPRESS_UPLOAD_MAX_SIZE 8M

RUN echo "file_uploads = On\n" \
        "memory_limit = ${WORDPRESS_UPLOAD_MAX_SIZE}\n" \
        "upload_max_filesize = ${WORDPRESS_UPLOAD_MAX_SIZE}\n" \
        "post_max_size = ${WORDPRESS_UPLOAD_MAX_SIZE}\n" \
        "max_execution_time = 600\n" \
        > /usr/local/etc/php/conf.d/uploads.ini

EXPOSE 80