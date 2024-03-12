# Projeto Integrador - Implantação De Banco De Dados

Nomes: 	LUIZ FELIPE MENDES GUIMARÃES
	WALLACE PEREIRA DE SOUZA
	YAGO WESLEY DA SILVA BATISTA


## Introdução



	Temos por finalidade deste projeto integrador trazer uma aplicação capaz de inovar na forma como estacionamentos funcionam, fazendo assim com eficiência e menos custos ao estabelecimento

	melhorias internas tanto para o usuário quanto para o proprietário do estabelecimento sendo ele um estacionamento(CNPJ) ou uma vaga residencial(CPF).


## Usos

	
	O uso final deste projeto é trazer dados às aplicações, para a melhor execução da tarefa solicitada sendo ela neste caso o melhor local para o usuário. Para executar e estudar precisa-se de:


- Modelo Conceitual [BrModelo](https://www.brmodeloweb.com/lang/pt-br/index.html)

- Banco De Dados [MySQL](https://www.mysql.com)

- Caderno de anotações [notepad++] (https://notepad-plus-plus.org)



### Para alimentar os dados é necessário utilizar sub-linguas do SQL, sendo elas:


	DDL: CREATE(cria no banco de dados uma tabela ou coluna), ALTER(altera as características de uma tabela existente e de suas colunas) e DROP(responsável por descartar um banco de dados, tabela ou coluna)

	DML: INSERT(insere informações em uma linha sempre em ordem com as colunas), UPDATE(atualiza valores das linhas) e DELETE(apaga informações indesejadas das linhas).


### Utilizando na prática com códigos

	DDL:

	CREATE TABLE USUARIOS (

	USUARIO\_CPF VARCHAR(18) NOT NULL,

	NOME VARCHAR(100) NOT NULL,

	EMAIL VARCHAR(25) NOT NULL,

	CELULAR VARCHAR(15),

	PRIMARY KEY (USUARIO\_CPF)

	);


	ALTER TABLE USUARIOS

	MODIFY COLUMN CELULAR VARCHAR(20);


	DROP TABLE USUARIOS;


	DML:

	INSERT INTO usuarios VALUES("421.235.098-76", "Luis Felipe M Guimaraes", "LuizFMG@live.com","1299735487");

	INSERT INTO usuarios VALUES("411.985.013-86", "Yago", "yago@live.com","4814615445");

	INSERT INTO usuarios VALUES("454.242.123-99", "Wallace Souza", "wallacesouza@live.com","4815441215");


	UPDATE USUARIOS SET USUARIO\_CPF = '464.242.124-33' WHERE CPF = '454.242.123-99';

	UPDATE USUARIOS SET NOME = 'Luiz' WHERE NOME = 'Luis';



	DELETE FROM USUARIOS WHERE USUARIO\_CPF = '454.242.123-99';
