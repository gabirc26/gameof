<h1 align="center">⚔ 🦁 🐺 Game of Thrones 🐻 🐲 🛡</h1>

Trabalho em grupo Módulo 4 do curso Programadores Cariocas.

Proposta do trabalho: A Resilia está pensando em lançar um novo sistema de acompanhamento e para isso precisa de ajuda para modelar um banco de dados que vai armazenar seus cursos, turmas e alunos. Para apoiar nesse sistema recebemos a tarefa de realizar essa modelagem e responder algumas perguntas com nosso modelo:

Resolução:
Existem outras entidades além dessas três?
Sim. No modelo criado para a solução deste minimundo, foi criado também a entidade "Resilia".

Quais são os principais campos e tipos?
Entidade Resilia( id_resilia serial primary key, campus varchar(20) not null );

Entidade Cursos( id_curso serial primary key, nome varchar(20) not null, coordenador );

Entidade Turmas( id_turmas serial primary key, qtd_alunos int );

Entidade Alunos( id_alunos serial primary key, nome varchar(30) not null, idade int not null, rg varchar(11) not null );

Como essas entidades estão relacionadas?
Segue imagem representando o modelo desde BD:

As perguntas:

*Quais são as 5 maiores notas da primeira temporada ordenadas de forma decrescente*

*Personagens que apareceram na série mais de 60 vezes*

*Dentre os 832 personagens, quais pertencem a casa Stark*

*Quais episódios começas com a palavra "The"? Qual a duração total desses episódios? Qual é o tempo do maior e o tempo do menor?*
Cardinalidade:

Resilia pode fornecer um ou vários cursos;

Curso pertence a um e somente um Resilia;

Curso pode produzir uma ou várias turmas;

Turma pertence a um e somente um curso;

Turma contém um ou vários alunos;

Alunos contém um ou vários cursos.

Registros:

Tabela Resilia:

registro resilia

Tabela Cursos:

registro cursos

Tabela Turmas:

registro turmas

Tabela Alunos:

registro alunos

🔧 Tecnologias utilizadas
SQL SHELL (psql)
🤝 Colaboradores
Devair Martins, Gabriela Rocha, Filipe Rodrigues e Thiago Máximo.

🎯 Status do projeto
Projeto finalizado.
