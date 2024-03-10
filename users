# Use Ubuntu 20.04 LTS as the base image
FROM ubuntu:20.04

# Create the 'collin' user with UID 5000
RUN useradd -m -u 5000 -s /bin/bash collin

# Create the /structure directory with appropriate permissions and files
RUN mkdir /structure && \
    chmod 777 /structure && \
    touch /structure/sync-work /structure/nobody-work && \
    chown sync /structure/sync-work && \
    chown nobody /structure/nobody-work

# Default command to keep the container running
CMD ["sh", "-c", "sleep infinity"]
