# rode a partir da imagem do node na versão 14;
FROM node:14-alpine
# exponha a porta 3001;
EXPOSE 3001
# adicione o arquivo node_modules.tar.gz à imagem;
WORKDIR /app
ADD node_modules.tar.gz .
# copie todos os arquivos da pasta back-end para a imagem. (você pode usar o caminho relativo, lembrando que a Dockerfile está em ./docker/todo-app/back-end/Dockerfile);
COPY . .
RUN npm install
# inicie a aplicação com o comando npm start respeitando as seguintes restrições:
  # ao subir um container baseado na imagem buildada a partir desse Dockerfile, o comando npm deve ser rodado sempre;
  # ao subir um container baseado na imagem buildada a partir desse Dockerfile, deve ser possível sobrescrever o comando start.
ENTRYPOINT ["npm"]
CMD [ "start" ]
