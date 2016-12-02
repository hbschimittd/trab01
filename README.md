# TRABALHO 01
Trabalho desenvolvido durante a disciplina de BD1

#Sumário

###1	COMPONENTES<br>

Hélio Braga Schimittd<br>

###2	INTRODUÇÃO E MOTIVAÇAO<br>

Este documento contém a especificação de uma aplicação que será usada para a diciplina de banco de dados.  <br>

###3	MINI-MUNDO<br>

Criar uma aplicação com integração com banco de dados. Essa aplicação será resposável basicamente por monitorar e acompanhar a evolução do usuario durante os treinos, entregando resultados de calculos especificos resultante dos valores gerados durante a evolução, mostrantando dicas de exercicío, alimentares e sugestões para facilitar a melhora nos resultados. <br>

###4	RASCUNHOS BÁSICOS DA INTERFACE (MOCKUPS)<br>
![Alt text](https://github.com/hbschimittd/trab01/blob/master/moc%201.png "Title")
![Alt text](https://github.com/hbschimittd/trab01/blob/master/mocf.png "Title")

###5 MODELO CONCEITUAL<br>
![Alt text](https://github.com/hbschimittd/trab01/blob/master/conceitual1.jpg "Title")

####5.1 Validação do Modelo Conceitual

    [Grupo01]: [Cassiano Künsch das Neves]
    [Grupo02]: [Romildo Costa & Pedro Henrique Elias da Cruz Costa]
    
###5.2 DECISÕES DE PROJETO

- Foi sugerida uma ideia pelo professor de criar mais uma outra entidades COMENTARIO, para gerar uma maior interação entre usuairos e para otimizar as apricações sobre os assuntos discutidos nos comentarios.

###5.3 DESCRIÇÃO DOS DADOS

TABLE USUARIO: Tabela que guarda os dados cadastrais do usuario.
- NOME: Guarda o nome do usuário
- SEXO: Guarda o sexo do usuário.
- D_NASCIMENTO: Gauarda a data de nascimento do usuário.
- E_MAIL: Guarda o e_mail o usuário.

TABLE FICHA: Tabela que guarda os dados que podem variar durante o perio da ficha.
- PESO: Guarda o peso do usuário.
- ALTURA: Guarda o altura do usuário.
- QUADRIL: Guarda o tamanto do quadril do usuário.
- FREQUENCIA: Guarda a freqencia com que o usuário pratica o exercício.
- D_INICIO: Guarda a data de inicil da ficha.
- D_FINAL: Guarda a data de finalização da ficha.

TABLE FICHA_EXERCICIO: Tabela que guarda as informações de execução dos exercícios da ficha.
- QUATIDADE: Guarda a quantidade de vezes o exercício sera executado.
- SERIE: Guarda quantas vezes as series do exercício sera executada.

TABLE EXERCICIO: Tabela guarda informações mais especificas sobre o exercício.
- NOME: Guarda o nome do exercicio.
- IMAGEM: Guarda uma imagem so exercício.

TABLE USUARIO_AVALIACAO: Tabela guarda os resultados obitidos ao decorres do tempo de execução de uma ficha.
- D_CONSULTA: Guarda a data de consulta dos resultados.
- IMC: Guarda o Índice de massa corporal para a data de consulta.
- GCD: Guarda o Gasto Calórico Diário para a data de consulta.
- IAC: Guarda o Índice de Adiposidade Corporal para a data de consulta.
- TBM: Guarda o Taxa Metabólica Basal para a data de consulta.
- PESO: Guarda o peso para a data de consulta.

TABLE COMENTARIO: Guarada as informações sobre o comentario feito entre usuários.
- ASSUNTO: Guarda o assunto principal do comentario.
- DATA_COMENT: Guarda a data que o comentario foi feito.

TABLE MENSAGEM: Guarda o conteudo do comentario feito entre usuários.
- TEXTO: Guarda o texto da mensagem.

TABLE RESPOSTA: Guarda as informações sobre a resposta dada por um usuário.
- TEXTO_R: Guarda o texto da resposta.
- DATA_R: Guarada a data em que a resposta foi enviada. 

###6 MODELO LÓGICO
![Alt text](https://github.com/hbschimittd/trab01/blob/master/logico1.jpg "Title")

###7 MODELO FÍSICO

https://github.com/hbschimittd/trab01/blob/master/total

###8 INSERT APLICADO NAS TABELAS DO BANCO DE DADOS

###8.1 DETALHAMENTO DAS INFORMAÇÕES

    Detalhamento sobre as informações e processo de obtenção ou geração dos dados.
    Referenciar todas as fontes referentes a :
    a) obtenção dos dados
    b) obtenção de códigos reutilizados
    c) fontes de estudo para desenvolvimento do projeto
    
###8.2 INCLUSÃO DO SCRIPT PARA CRIAÇÃO DE TABELA E INSERÇÃO DOS DADOS

https://github.com/hbschimittd/trab01/blob/master/insert
    
###9 TABELAS E PRINCIPAIS CONSULTAS

###9.1 CONSULTAS DAS TABELAS COM TODOS OS DADOS INSERIDOS (Todas) 

SELECT * FROM USUARIO;
https://github.com/hbschimittd/trab01/blob/master/select1.png

SELECT * FROM FICHA;
https://github.com/hbschimittd/trab01/blob/master/select2.png

SELECT * FROM FICHA_EXERCICIO;
https://github.com/hbschimittd/trab01/blob/master/select3.png

SELECT * FROM EXERCICIO;
SELECT * FROM USUARIO_AVALIACAO;
SELECT * FROM COMENTARIO;
SELECT * FROM MENSAGEM;
SELECT * FROM RESPOSTA;

###9.2 CONSULTAS DAS TABELAS COM FILTROS WHERE (Mínimo 3)

https://github.com/hbschimittd/trab01/blob/master/WHERE

###9.3 CONSULTAS QUE USAM OPERADORES LÓGICOS, ARITMÉTICOS E CAMPOS RENOMEADOS (Mínimo 2)

https://github.com/hbschimittd/trab01/blob/master/OPERADORES%20LOGICOS

###9.4 CONSULTAS QUE USAM OPERADORES LIKE (Mínimo 3) 

https://github.com/hbschimittd/trab01/blob/master/LIKE

###9.5 ATUALIZAÇÃO E EXCLUSÃO DE DADOS (Mínimo 6)

https://github.com/hbschimittd/trab01/blob/master/UPDATE

###9.6 CONSULTAS COM JUNÇÃO E ORDENAÇÃO (Todas Junções)

    Entrega até este ponto em 22/11/2016
    
###9.7 CONSULTAS COM GROUP BY (Mínimo 5)

https://github.com/hbschimittd/trab01/blob/master/GROUP%20BY

###9.8 CONSULTAS COM LEFT E RIGHT JOIN (Mínimo 4)

###9.9 CONSULTAS COM SELF JOIN E VIEW (Todas Possíveis)

###9.10 SUBCONSULTAS (Mínimo 3)

    Entrega até este ponto em 29/11/2016
    
###10 ATUALIZAÇÃO DA DOCUMENTAÇÃO DOS SLIDES PARA APRESENTAÇAO FINAL (Mínimo 6 e Máximo 10)

###11 DIFICULDADES ENCONTRADAS PELO GRUPO

Algumas dificuldades no entendimento do trabalho foram apresentadas, mas com a percistencia na execução e com pesquisas as duvidas foram sendo sanadas. No entanto ainda se aprensentava duvidas na estruturação do mesmo, mas também foram solucionadas.

###12 FORMATACAO NO GIT: https://help.github.com/articles/basic-writing-and-formatting-syntax/

