#
 
#
# The line below states we will base our new image on the Latest Official Ubuntu 
FROM ubuntu:latest
 
#
# Identify the maintainer of an image
LABEL maintainer="vishalgeniuss@gmail.com"
 
#
# Update the image to the latest packages
RUN apt-get update && apt-get upgrade -y
 
#
# Install NGINX to test.
RUN apt-get install nginx -y

RUN echo "This is our new Nginx Test Site by Vishal Arora" >> /var/www/html/index.html 

#
# Expose port 80
EXPOSE 80
 
#
# Last is the actual command to start up NGINX within our Container
CMD ["nginx", "-g", "daemon off;"]
