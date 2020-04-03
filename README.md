<img style="align:center;" src="/images/docker.jpg">

# 🐋 Curso-Docker by Cod3r

#### Dockerfile e docker-compose.yml que fiz durante o curso de docker da cod3r

## 👨🏽‍💻 Comandos

#### Abaixo alguns comandos que anotei

``` bash
$ Comando run sempre cria um novo container.

$ Para dar um nome a um novo container é necessário para a flag --name nome-do-container

$ -i inicia no modo interativo -t entra no container

$ -it para entrar no container em modo interativo

$ -a ter acesso ao terminal

$ docker container ou docker start inicia o container já criado

$ -p 8080:80 o primeiro 8080 é a porta que vai ser exportada e para acessar o serviço dentro do container,e a porta 80 é onde o serviço vai rodar

$ mapear volume -v a pasta do host que eu quero mapear: a pasta dentro do container

$ docker container run -p 8080:80 -v $(pwd):/usr/share/nginx/html nginx

$ -d significa que vai rodar o container no modo daemon, vai ficar em backgroud apenas para utilizar o que está dentro

$ docker image pull - baixa imagem do docker hub, pode acontecer implicitamente por exemplo no docker run, se a imagem não existe na máquina ele vai la e baixa

$ docker image ls - mostra as imagens salvas na máquina

$ docker image rm - para remover imagem

$ docker imagem inspect - mostra um json com info sobre as imagens

$ docker image tag {image} {tag} - adiciona uma tag a imagem, como --name ao container

$ docker image build - pegar um arquivo descritor do docker e gerar imagem

$ docker image push - para publicar uma imagem no register local da empresa ou no hub 

$ docker registry: serviço server side, para registro e obtenção de imagens(é uma api).

$ docker hub: é um SaaS, contém um registry dentro dele , interface gráfica e maior. 

$ docker image build -t ex-simple-build . -t para dar uma tag para essa image dps a tag, depois a pasta onde achar o dockerfile

$ docker image tag ex-simple-build cristuker/simple-build:1.0 - criando uma tag para uma imagem que já tenho salvar e referenciado ao meu usuário

$ docker login --username=cristuker - para logar no docker pelo terminal

$ docker container run --rm --net none alpine ash-c “ifconfig” --] --net é onde vc passa o seu tipo de rede e o --rm é para remover o container assim que terminar de rodar

$ -d deixa rodando em modo deamon

$ docker container exec -it container1 ping 172.17.0.3 -- pinga do container 1 para o container 2, mas nesse caso para pingar no container 2 é necessario passar o io dele

$ docker network create --driver birdge rede_nova - eu crio uma nova rede com base no driver bridge e nomeio ela de rede_nova
```

Fiz algumas anotação de comando durante o curso e irei deixar aqui compartilhadas

Made with ♥ by [Cristian Silva](https://www.linkedin.com/in/cristian-silva-dev/)