FROM centos:7

# Install prepare infrastructure
RUN yum -y update && \
 yum -y install wget && \
 yum clean all

WORKDIR /tmp/openfire
RUN wget -O ./openfire-4.2.2-1.x86_64.rpm 'https://www.igniterealtime.org/downloadServlet?filename=openfire/openfire-4.2.2-1.x86_64.rpm'
RUN rpm -ivh openfire-4.2.2-1.x86_64.rpm

CMD ["/opt/openfire/bin/openfire.sh"]
