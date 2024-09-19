# Usar uma imagem oficial do Node.js como base
FROM node:16

# Definir o diretório de trabalho dentro do contêiner
WORKDIR /app

# Copiar o arquivo package.json e instalar as dependências
COPY package.json /app/
RUN npm install --only=production

# Copiar o restante do código para o contêiner
COPY . /app/

# Expor a porta que o React usará
EXPOSE 3000

# Comando para iniciar a aplicação React
CMD ["npm", "start"]