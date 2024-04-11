# pdv-php

O presente sistema tem o objetivo de testar meus conhecimentos. Utilizando apenas PHP para o backend, foi desenvolvido um sistema onde se possa cadastrar produtos, seus tipos e fazer vendas.

# Instalação

Na raz do projeto, está disponível um arquivo docker-compose.yml, que está configurado para rodar todo o sistema, incluindo o backend, frontend e o banco de dados.
Para se conectar ao banco de dados, a pasta do backend contém um arquivo .env.example, que necessita ser copiado e renomeado para .env. Lá é possível alterar as credenciais de acesso ao banco.

Caso o Docker não seja uma opção, a instalação nativa também é bem simples:

Para o backend, é necessário apenas o PHP8 com a extensão pdo_pgsql habilitada, sem precisar rodar composer install por exemplo.
Com a extensão habilitada, basta rodar php -S (host:porta) para iniciar o servidor php.

Para o frontend, é necessário o Node na versão 17+. Neste caso, é necessário instalar o Angular utilizando o comando: npm install -g @angular/cli@16.0.0
Após a instalação, será necessário também rodar o comando npm install.
Finalizando, será necessário rodar ng add @angular/material.
Após isso, para servir a aplicação, basta rodar ng serve.

Para o banco de dados, no repositório do backend, está presente um arquivo dump.sql que pode ser rodado para popular o banco com dados iniciais.
