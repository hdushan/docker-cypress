FROM cypress/browsers:node12.13.0-chrome80-ff74

COPY package.json ./package.json

RUN npm install --quiet --global && \
    npm cache clean --force && \
    npm bin && \
    ./node_modules/.bin/cypress verify