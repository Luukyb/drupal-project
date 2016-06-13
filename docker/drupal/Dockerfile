FROM drupal:8

RUN apt-get update -qq \
  && apt-get install wget mysql-client -yq

RUN usermod -u 1000 www-data

RUN wget -O /usr/local/bin/drush http://files.drush.org/drush.phar \
  && chmod +x /usr/local/bin/drush
RUN drush core-status
