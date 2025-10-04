FROM rockylinux:8
RUN yum -y update && \
    yum -y install python3 iputils && \
    yum clean all
WORKDIR /app
COPY index.html /app/index.html
EXPOSE 80
CMD ["python3", "-m", "http.server", "80"]
