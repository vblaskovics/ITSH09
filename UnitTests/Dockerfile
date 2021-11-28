# Init base image
FROM ubuntu
# Install node
RUN apt-get update
RUN apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_12.x | bash -
RUN apt-get install -y nodejs
# Install git and clone repo
RUN apt update
RUN apt install -y git
RUN git clone https://github.com/MarcL/js-unit-testing-examples.git js-unit-testing-examples
# Init and run app
WORKDIR /js-unit-testing-examples
RUN npm install
CMD npm test
