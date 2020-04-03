FROM nginx:latest
LABEL maintainer 'Cristian'

RUN echo '<h1>Sem conteudo</h1><script>alert("oi")</script>' > /usr/share/nginx/html/conteudo.html
COPY *.html /usr/share/nginx/html/
RUN apt-get update
RUN apt-get -y install curl gnupg
RUN curl -sL https://deb.nodesource.com/setup_11.x  | bash -
RUN apt-get -y install nodejs
RUN node -v
COPY *.js /usr/share/nginx/html/
RUN cd /usr/share/nginx/html/ && node index.js 