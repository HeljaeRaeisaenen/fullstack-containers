FROM node:24

WORKDIR /usr/src/counter-app

COPY --chown=node:node . .

RUN npm ci --omit=dev

USER node

ENV DEBUG=express:*

CMD ["npm", "start"] 
