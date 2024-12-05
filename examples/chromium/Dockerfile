FROM cypress/base
COPY . /opt/app
WORKDIR /opt/app
RUN apt-get update              # Update package index
RUN apt-get install chromium=130.0.6723.91-1~deb12u1 chromium-common=130.0.6723.91-1~deb12u1 -y # Install older Chromium
RUN npx cypress install         # Install Cypress binary
