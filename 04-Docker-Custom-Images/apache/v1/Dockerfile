# Base Images 
FROM ubuntu:noble 

# Owner Detials 
MAINTAINER Amit Vashistha < amitvashist.tech@gmail.com> 

# Update APT Repo
RUN apt-get update 

# Install Apache 2 Web Package 
RUN apt-get install apache2 -y 

# Execute the Service 
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND" ]
