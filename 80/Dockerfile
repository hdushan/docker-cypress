FROM cypress/browsers:node13.6.0-chrome-80-ff72

COPY package.json ./package.json

RUN npm install --quiet --global && \
    npm cache clean --force