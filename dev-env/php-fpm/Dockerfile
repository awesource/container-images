FROM phpdockerio/php7-fpm:latest

# Install selected extensions and other stuff
RUN apt-get update \
    && apt-get -y --no-install-recommends install  php7.0-memcached php7.0-mongodb php7.0-mysql php7.0-redis php7.0-sqlite3 php7.0-bz2 php7.0-gd php7.0-intl php7.0-tidy \
    && apt-get clean; rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*


WORKDIR "/var/www/unitics-core"