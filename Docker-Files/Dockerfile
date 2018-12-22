FROM corentinaltepe/heirloom-mailx
RUN apk update
RUN apk add postfix
RUN  mkfifo /var/spool/postfix/public/pickup
COPY test.sh /opt/test.sh
RUN chmod 777 /opt/test.sh
ENTRYPOINT /usr/sbin/postfix start && echo "Docker" | mailx -s 'Docker test' chetan.pachare@widas.in &&  sleep 60
#CMD /opt/test.sh
