# This Dockerfile will create a image for our spring based java applications 
# Base image 

FROM openjdk:18.0.2.1-jdk
RUN mkdir -p /opt/i27/
ARG JAR_SOURCE
WORKDIR /opt/i27/
COPY ["${JAR_SOURCE}", "/opt/i27/i27cart-product.jar"]
RUN chmod 777 /opt/i27/
EXPOSE 8132
CMD ["java", "-jar", "/opt/i27/i27cart-product.jar"]

# /opt/i27/i27cart-product.jar > will be in the container 
