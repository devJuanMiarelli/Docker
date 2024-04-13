# Como execução destas aplicações utilizando Docker

* ARQUITETURA:

![image](https://github.com/aannddrree/ProjectOnlineDocker/assets/8753843/455d8b3a-827e-4be7-9574-2926f4bec380)


* APP JAVA SPRINGBOOT:

Acessar o diretório "projTest" via terminar e executar:

```
docker build -t aplicacao_spring .
```

```
docker run --name java-container-test -d -p 8081:8080 aplicacao_spring 
```

* PAGINA HTML (SERVER NGINX):

```
docker build -t nginx .
```

```
docker run --name app-web -d -p 8080:80 nginx 
```

* APOS EXECUTAR:

```
docker image list
```

![image](https://github.com/aannddrree/ProjectOnlineDocker/assets/8753843/23ee726e-e975-455a-a6d3-04f35eedd3ca)

```
docker ps
```

![image](https://github.com/aannddrree/ProjectOnlineDocker/assets/8753843/d8f13b95-c961-41fc-a458-51325b9a94bd)

* RESULTADO:

![image](https://github.com/aannddrree/ProjectOnlineDocker/assets/8753843/62cd95bb-1948-48fc-8f36-cd9236a25933)

![image](https://github.com/aannddrree/ProjectOnlineDocker/assets/8753843/49802b91-6bf1-4d8c-a462-12c673567eab)
