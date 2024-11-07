# Usar uma imagem base leve do Node.js
FROM node:14-alpine

# Definir diretório de trabalho dentro do container
WORKDIR /app

# Copiar o arquivo package.json e o package-lock.json
COPY package*.json ./

# Instalar as dependências
RUN npm install

# Copiar o restante do código da aplicação
COPY . .

# Compilar o código React
RUN npm run build

# Expor a porta 3000 para o servidor web
EXPOSE 3000

# Comando para iniciar a aplicação
CMD ["npm", "start"]

