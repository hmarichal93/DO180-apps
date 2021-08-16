FROM ubi7/ubi:7.7
MAINTAINER Gonzalo gvallarino@isbel.com.uy
LABEL description="A custom Apache container based on UBI 7"
RUN yum install -y httpd && \
yum clean all
RUN echo "Hello from Dockerfile" > /var/www/html/index.html
#The EXPOSE instruction does not actually make the specified port available to the
#host; rather, the instruction serves as metadata about which ports the container is
#listening on.
EXPOSE 80
CMD ["httpd", "-D", "FOREGROUND"]

