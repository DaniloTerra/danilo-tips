# Download Composer
- curl -sS https://getcomposer.org/installer | php
- php -r "readfile('https://getcomposer.org/installer');" | php

# Criar projeto usando Composer
- composer create-project laravel/laravel --prefer-dist [nomeDoDiretorio]

#Iniciar servidor PHP
- php artisan serve

# Instalar pacotes Bower
- bower install

# Autoload de classes do Laravel
- php artisan dump-autoload
- composer dump-autoload

# Servidor PHP embutido > PHP 5.4
- php -S localhost:8000
