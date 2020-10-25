# docker/build/apache/Dockerfile

#FROM httpd:2.4
FROM php:7.4-apache


# Copy Symfony files: COPY [FROM_MACHINE] [TO_CONTAINER]
      # COPY test.txt copied-test.txt                               <- Remove this line (and also the text.txt file!)
      # COPY . ./htdocs                                             <- Remove this


# <- Keep attention: we have removed the "." (dot) at the beginning of the destination path
COPY . /var/www/html/
RUN  chmod a+rwx -R /var/www/html/var/cache
RUN  chmod a+rwx -R /var/www/html/var/log

