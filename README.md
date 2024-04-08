
# teste_imagem
# Use uma imagem base
FROM ubuntu:latest

# Instale as dependências necessárias
RUN apt-get update && apt-get install -y <pacote1> <pacote2> ...

# Copie os arquivos do seu projeto para o contêiner
COPY . /app

# Defina o diretório de trabalho
WORKDIR /app

# Especifique o comando padrão a ser executado quando o contêiner for iniciado
CMD ["./start.sh"]
