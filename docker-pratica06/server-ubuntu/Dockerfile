FROM ubuntu:22.04
ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update && \
    apt-get install -y python3 iputils-ping curl && \
    rm -rf /var/lib/apt/lists/*
WORKDIR /app
COPY index.html /app/index.html
EXPOSE 80
CMD ["python3", "-m", "http.server", "80"]
