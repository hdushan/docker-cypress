FROM cypress/browsers:node16.5.0-chrome94-ff93

COPY package.json ./package.json

ENV NODE_PATH=/node_modules/

RUN npm install --quiet && \
    npm cache clean --force && \
    npm bin && \
    npx cypress verify && \
    npx browserslist@latest --update-db