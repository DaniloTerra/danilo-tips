# Descompactar arquivos .tar.gz
- tar xzf file.tar.gz
- tar xzvf file.tar.gz (para acompanhar o processo de extração)

# Instalar aquivos .sh
- chmod +x nomeDoArquivo.sh
- ./nomeDoArquivo.sh

# Excluir um arquivo
- rm /home/danilo/arquivo.txt

#Aumentar velocidade do Mouse
- xset m 2 1

# Alterrar o nome do diretório
- mv /home/danilo/vhosts/nome-do-projeto /home/danilo/vhosts/novo-nome

# Download Composer
- curl -sS https://getcomposer.org/installer | php
- php -r "readfile('https://getcomposer.org/installer');" | php

# Criar projeto usando Composer
- composer create-project laravel/laravel --prefer-dist [nomeDoDiretorio]

# Instalar pacotes Bower
- bower install

#Iniciar servidor PHP
- php artisan serve

# Autoload de classes do Laravel
- php artisan dump-autoload
- composer dump-autoload

# Servidor PHP embutido > PHP 5.4
- php -S localhost:8000

# Verificar os processos que estão abertos na porta 80/TCP
- sudo fuser -v 80/tcp
- sudo fuser -n tcp 8000

# Matar o processo aberto em determinada porta
- kill -9 "PID_NUMBER"

# Remover todos os diretórios e subdiretórios, com seu conteúdo
- rm -rf /home/data/2000

# Instalar o servidor HTTP do NodeJs
- npm install http-server -g

# Iniciar o servidor HTTP do NodeJS
- Na raiz do projeto digitar: http-server ./

# Visualizar o conteúdo de um arquivo diretamente no terminal
- cat nomeDoArquivo.extensao

# Instalar o gulp no seu projeto
- npm install gulp --save-dev

# Criar um branch no GIT
- git branch nomeDoBranch

# Mudar de branch no GIT
- git checkout nomeDoBranch

# Fazer merge no branch atual
- git merge nomeDoBranchASerMescladoComOAtual

# Excluir branch no GIT
- git branch -d nomeDoBranchASerExcluido
