FROM cypress/browsers:node14.17.0-chrome91-ff89

COPY package.json ./package.json

RUN npm install --quiet --global && \
    npm cache clean --force && \
    npm bin && \
    ./node_modules/.bin/cypress verify