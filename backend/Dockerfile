# Usar uma imagem base do Node.js
FROM node:14

# Definir diretório de trabalho dentro do container
WORKDIR /app

# Copiar o arquivo package.json e o package-lock.json
COPY package*.json ./

# Instalar as dependências
RUN npm install

# Copiar o restante do código da aplicação
COPY . .

# Expor a porta 5000 para a API
EXPOSE 5000

# Comando para iniciar a aplicação
CMD ["node", "server.js"]
