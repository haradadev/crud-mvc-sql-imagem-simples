# crud-mvc-sql-imagem-simples
 Criar a pasta em HTDOCS: crud-mvc-sql-imagem-simples

#CRIANDO A ESTRUTURA BÁSICA DO MVC
Abrir o VSCode:
1- Selecionar pasta crud-mvc-sql-imagem-simples 
2- Abrir o terminal do VSCode e colar o código abaixo:

mkdir app
mkdir img
mkdir app\config
mkdir models
mkdir controllers
mkdir views

New-Item index.php -ItemType File
New-Item app\config\conexao.php -ItemType File
New-Item models\Usuario.php -ItemType File
New-Item controllers\UsuarioController.php -ItemType File
New-Item views\listar.php -ItemType File
New-Item views\criar.php -ItemType File
New-Item views\editar.php -ItemType File

#Banco de dados:

CREATE DATABASE bd_loja_mvc;
USE bd_loja_mvc;

CREATE TABLE usuario (
    id INT AUTO_INCREMENT PRIMARY KEY,
    nome VARCHAR(100),
    email VARCHAR(100),
    imagem VARCHAR(255),
    login VARCHAR(50),
    senha VARCHAR(100)
);



