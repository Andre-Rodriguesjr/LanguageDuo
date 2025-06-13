# LanguageDuo
Site feito para a aula de  Linguagem Técnica de Programação Web, o site é sobre um curso de idiomas, onde a pessoa pode escolher o idioma e com quem quer fazer as aulas.

Abaixo está os codigos do Banco de dados do site

create database languageduo;

use languageduo;


create table Usuario(
id int primary key auto_increment,
nome varchar(100),
email varchar(100),
senha varchar(100)
);

create table aula(
id int primary key auto_increment,
data_ varchar(100),
hora varchar(100),
curso varchar(100),
duracao varchar(100)
);



select * from aula;
select * from Usuario;  e as tabelas de antes pra usar e funcionar o array, cadastro...

SELECT 
    a.id AS aula_id,
    a.data_,
    a.hora,
    a.curso,
    a.duracao,
    u.nome AS nome_usuario,
    u.email
FROM aula a
JOIN Usuario u ON a.id = u.id; tem esse join que funciona meia boca
