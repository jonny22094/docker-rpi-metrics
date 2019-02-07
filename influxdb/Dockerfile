FROM influxdb

# Set the working directory to /usr/src/app:
WORKDIR /usr/src/app

# Copy all the config files from the host's directory to /docker/bin container
# directory:
COPY metrics/influxdb/influxdb.conf /etc/influxdb/influxdb.conf

# Docker usually inherits file permissions from host, so we have to ensure that
# copied files will be able to be executed:
RUN chmod -R +x /etc/influxdb/influxdb.conf
