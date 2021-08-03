FROM node:lts-buster

ARG init

WORKDIR /usr/src/app/src

EXPOSE 80

RUN /bin/bash -c 'if [[ -z "$init" ]] ; then echo "Project initialized ..." ; else npm install -g moleculer-cli && npm i moleculer; fi' 
#  && npx --yes moleculer-cli -c moleculer init project src

CMD ["npm", "run", "dev"]