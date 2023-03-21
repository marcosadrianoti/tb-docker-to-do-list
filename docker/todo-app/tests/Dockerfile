# rode a partir da imagem do mjgargani/puppeteer:trybe1.0;
FROM mjgargani/puppeteer:trybe1.0
# adicione o arquivo node_modules.tar.gz à imagem;
WORKDIR /app
ADD node_modules.tar.gz .
# copie todos os arquivos da pasta tests para a imagem. (você pode usar o caminho relativo, lembrando que a Dockerfile está em ./docker/todo-app/tests/Dockerfile);
COPY . .
RUN npm install
# inicie a aplicação com o comando npm test respeitando as seguintes restrições:
  # ao subir um container baseado na imagem buildada a partir desse Dockerfile, o comando npm deve ser rodado sempre;
  # ao subir um container baseado na imagem buildada a partir desse Dockerfile, deve ser possível sobrescrever o comando test.
ENTRYPOINT ["npm"]
CMD [ "test" ]
