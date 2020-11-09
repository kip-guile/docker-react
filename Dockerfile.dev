FROM node:alpine

WORKDIR '/app'

COPY ./package.json ./

RUN npm install
# if building for production, RUN npm ci --only=production

## Bundle app source
COPY . .

CMD ["npm", "run", "start"]