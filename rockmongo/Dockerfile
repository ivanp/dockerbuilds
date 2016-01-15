FROM kucing/php56

RUN curl -L -o /root/rockmongo.tgz https://github.com/iwind/rockmongo/archive/1.1.7.tar.gz && \
    mkdir -p /var/www && \
    tar -zx -C /var/www -f /root/rockmongo.tgz && \
    rm -fv /root/rockmongo.tgz

WORKDIR /var/www/rockmongo-1.1.7

EXPOSE 80
CMD php -S 0.0.0.0:80
