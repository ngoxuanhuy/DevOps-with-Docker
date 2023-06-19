# Start from the ubuntun 20.04 image
FROM ubuntu:20.04

# User /exercise1.7 as the working directory
WORKDIR /exercise1.7

# Copy the web-search.sh file from the local location to /exercise1.7 
COPY web-search.sh .

# Execute permissions during the build
RUN chmod +x web-search.sh

# Install curl
RUN apt-get update && apt-get install -y curl

# Execute the script when running docker
CMD ./web-search.sh