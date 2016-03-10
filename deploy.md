# Deploy passo-a-passo

## 1 - Clonar repositório no diretório /var/www

## 2 - Dentro do diretório criado, instalar pacotes composer

## 3 - Copiar .env.exemple para .env

## 4 - Gerar chave da aplicação pelo Artisan

## 5 - Mudar ownership do diretório para www-data
- sudo chown -R www-data /var/www/novoDiretorio

## 6 - Configurar novo arquivo em /etc/nginx/sites-available

## 7 - Fazer link simbólico para /etc/nginx/sites-enabled

## 8 - Reiniar Nginx

# Conectar-se a um servidor remoto usando SSH
- ssh usuarioRemoto@enderecoDoServidor

# Configurar o Virtual Host no Nginx

## 1º - Criar o arquivo de configuração no diretório 'sites-available' com base no arquivo exemplo
- cd /etc/nginx/sites-available/
- sudo cp default siteexemplo.com.conf

## 2º - Criar um link simbólico no diretório 'sites enabled' para o arquivo recém criado no diretório 'sites available'
- sudo ln -s /etc/nginx/sites-available/siteexemplo.com.conf /etc/nginx/sites-enabled/siteexemplo.com.conf

## 3º - Reiniciar o nginx
- sudo service nginx restart

## 4º - Alterar o arquivo /etc/hosts
- sudo gedit /etc/hosts

## Reiniciar o Nginx
- sudo service nginx restart

## Mudar o privilégio do diretório
- sudo chown -R www-data /var/www/novoDiretorio
- sudo chmod 755 /home/danilo/vhosts/diretorio

## Consultar os erros no NGINX (quando não dá para reiniciar ele)
- nginx -t
