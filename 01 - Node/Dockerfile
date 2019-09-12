#define a imagem base
FROM node:alpine

#define o diretorio base para rodar o app
WORKDIR /app

#copia primeiro somente o arquivo package.json para otimizar o build da imagem,
#ja que o comando npm install depende deste arquivo
COPY package.json .
RUN npm install
#copia os demais arquivos posteriormente para nao ter que instalar todo o npm em caso de mudanca no codigo fonte
COPY . .

#define o comando inicial
CMD ["npm", "start"]
