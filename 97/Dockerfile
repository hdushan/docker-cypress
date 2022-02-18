FROM cypress/browsers:node16.13.2-chrome97-ff96

COPY package.json ./package.json

ENV NODE_PATH=/node_modules/

RUN npm install --quiet && \
    npm cache clean --force && \
    npm bin && \
    npx cypress verify && \
    npx browserslist@latest --update-db