cat Dockerfile 
FROM centos:latest

# Update
RUN yum install gcc python git python-libs python-devel openssl-libs openssl-devel net-tools vim -y
RUN curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
RUN python get-pip.py
RUN pip install uwsgi
RUN pip install supervisor
RUN mkdir -p /etc/supervisor/conf.d
