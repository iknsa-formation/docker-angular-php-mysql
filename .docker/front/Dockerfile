FROM node:14.16

WORKDIR /home/node/app

RUN npm install -g @angular/cli

COPY ../../front/package.json .

RUN npm install && ng build && ng serve

CMD ["node"]