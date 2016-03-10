Deploy passo-a-passo
	1 - Clonar repositório no diretório /var/www
	2 - Dentro do diretório criado, instalar pacotes composer
	3 - Copiar .env.exemple para .env
	4 - Gerar chave da aplicação pelo Artisan
	5 - Mudar ownership do diretório para www-data
		sudo chown -R www-data /var/www/novoDiretorio
  6 - Configurar novo arquivo em /etc/nginx/sites-available
	7 - Fazer link simbólico para /etc/nginx/sites-enabled
	8 - Reiniar Nginx

Conectar-se a um servidor remoto usando SSH
	ssh usuarioRemoto@enderecoDoServidor
	ssh root@45.55.240.216

Configurar o Virtual Host no Nginx
	1º - Criar o arquivo de configuração no diretório 'sites-available' com base no arquivo exemplo
		cd /etc/nginx/sites-available/
		sudo cp default siteexemplo.com.conf

	2º - Criar um link simbólico no diretório 'sites enabled' para o arquivo recém criado no diretório 'sites available'
		sudo ln -s /etc/nginx/sites-available/siteexemplo.com.conf /etc/nginx/sites-enabled/siteexemplo.com.conf

	3º - Reiniciar o nginx
		sudo service nginx restart

	4º - Alterar o arquivo /etc/hosts
		sudo gedit /etc/hosts

Reiniciar o Nginx
	sudo service nginx restart

Mudar o privilégio do diretório
	sudo chown -R danilo:www-data /home/danilo/vhost/diretorio
	sudo chmod 755 /home/danilo/vhosts/diretorio

Clonar repositório
	git clone https://DaniloTerra@bitbucket/repositorio.git [nomeDoDiretorio]

Instalar pacotes Composer
	composer install

Instalar pacotes Npm
	sudo npm install

Criar .env
	cp .env.example .env

Gerar chave segura para o Laravel
	php artisan key:generate

Adicionar website no servidor
	1 - Clonar repositório
	2 - Mudar privilégios do repositório
		sudo chown -R danilo:www-data /var/www/projeto/
		sudo chmod 755 /var/www/projeto/storeage/
  3 - Instalar os componentes do composer
		composer install
  4 - Criar .env
		cp .env.example .env
	5 - Criar banco de dados
	6 - Rodar migrations
	7 - Gerar chave de encriptação
	8 - Criar arquivo de configuração em /etc/nginx/sites-available
	9 - Linkar o o arquivo em /etc/nginx/sites-enabled
		sudo ln -s /etc/nginx/sites-available/siteexemplo.com.conf /etc/nginx/sites-enabled/
	10 - Reiniciar nginx

Fechar a sessão corrente
	exit

Atualizar repositório no servidor online
	/var/www/repositorio
	php artisan down
	git pull origin master
	php artisan up
	sudo service nginx restart

Consultar os erros no NGINX (quando não dá para reiniciar ele)
	nginx -t
