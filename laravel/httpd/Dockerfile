FROM httpd:2.4.28
RUN sed -i \
-e "s/#LoadModule\ proxy_module/LoadModule\ proxy_module/g" \
-e "s/#LoadModule\ proxy_fcgi_module/LoadModule\ proxy_fcgi_module/g" \
-e "s/#LoadModule\ rewrite_module/LoadModule\ rewrite_module/g" \
/usr/local/apache2/conf/httpd.conf
RUN echo "Include conf/extra/httpd-fpm.conf\n" >> /usr/local/apache2/conf/httpd.conf 
ADD ./fpm.conf /usr/local/apache2/conf/extra/httpd-fpm.conf
