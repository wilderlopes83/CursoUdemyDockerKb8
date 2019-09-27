#comando para buildar o container
    docker build -t wilderlopes/simpleweb .

#comando para rodar o container, mapeando a porta 8080
    docker run -p 8080:8080 wilderlopes/simpleweb