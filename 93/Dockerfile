FROM cypress/browsers:node16.5.0-chrome94-ff93

COPY package.json ./package.json

RUN npm install --quiet --global && \
    npm cache clean --force && \
    npm bin && \
    ./node_modules/.bin/cypress verify