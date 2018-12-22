# In your Dockerfile
From centos

RUN yum update -y

RUN yum install -y sendmail
# Run mail listener
RUN sendmail -bd

CMD sleep infinity
# or run your command
