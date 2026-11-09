
FROM httpd:2.4.68

COPY dav.conf /usr/local/apache2/conf/extra/dav-lab.conf

RUN printf '\nInclude conf/extra/dav-lab.conf\n' \
    >> /usr/local/apache2/conf/httpd.conf \
    && mkdir -p /usr/local/apache2/htdocs/webdav \
                /usr/local/apache2/var \
    && chown -R www-data:www-data \
        /usr/local/apache2/htdocs/webdav \
        /usr/local/apache2/var
