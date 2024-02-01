# Projeto Docker Compose

Este projeto é constituído por três contêineres Docker: frontend, backend e um banco de dados MongoDB. Esses elementos se unem para criar uma aplicação web integrada e eficiente.

## Requisitos
- [Ubuntu](https://ubuntu.com)
- [Docker](https://www.docker.com/get-started/)

## Preparação do ambiente
### Instalação do Docker:

1. **Atualize seu sistema:**
   ```bash
   $ sudo apt update
2. **Remova versões antigas do Docker (se houver):**
   ```bash
   $ sudo apt remove docker docker-engine docker.io containerd runc
3. **Instale dependências:**
   ```bash
   $ sudo apt install apt-transport-https ca-certificates curl software-properties-common
4. **Adicione a chave GPG oficial do Docker:**
   ```bash
   $ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
5. **Adicione o repositório Docker ao APT sources:**
   ```bash
   $ sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
6. **Atualize o índice de pacotes do apt:**
   ```bash
   $ sudo apt update
7. **Instale o Docker:**
   ```bash
   $ sudo apt install docker-ce
8. **Verifique se a instalação foi bem-sucedida:**
   ```bash
   $ docker --version
9. **Teste sua instalação Docker:**
   ```bash
   $ docker run hello-world

## Como utilizar?
1- Clone o repositório.
```bash
$ git clone https://github.com/rocoxta/docker-compose-app.git
```
2- Construa as imagens Docker:
```bash
$ docker-compose build
```
## Execução
1- Inicie os serviços usando Docker Compose:
```bash
$ docker-compose up
```
## Acesso

- Frontend: http://localhost:3000
- Backend: http://localhost:3001
- Banco de dados MongoDB: mongodb://localhost:27017/vidly

## Observações
- Certifique-se de que as portas 3000, 3001 e 27017 não estejam sendo utilizadas por outros serviços.
- As imagens Docker serão construídas automaticamente durante a primeira execução do Docker Compose.
- Para parar a execução dos serviços, pressione Ctrl+C no terminal onde o Docker Compose está em execução.
- DB_URL: URL de conexão com o banco de dados. (Padrão: mongodb://db/vidly)

## Referências
- [Docker Install](https://docs.docker.com/engine/install/)
- [Docker Compose](https://docs.docker.com/compose/)
## Autor
👤 **Rodrigo Costa**
