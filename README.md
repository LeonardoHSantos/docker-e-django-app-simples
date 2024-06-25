# Aplicação Django simples com foco na utilização de container Docker.

#### Documentação oficial Docker
- https://docs.docker.com/guides/

#### Documentação para gerar a imagem Docker utilizada
- https://hub.docker.com/_/django

### Arquivos e configurações
1) Rodei o projeto usando WSL 2 (Ambiente Linux dentro do sistema Windows)

2) criar esse arquivos:
- Dockerfile ----> utilizado para configuração da imagem;
- docker-compose.yml ----> arquivo auxiliar para mapear portas e comandos Python.

### Gerando a imagem
<pre>
docker build -t nome_do_responsavel/nome_da_imagem:versao_da_imagem .
</pre>

### Ativando a imagem
<pre>
docker run --name some-django-app -d my-django-app
</pre>

### Rodando o app Django com Docker 
<pre>
docker-compose up -d --build
</pre>