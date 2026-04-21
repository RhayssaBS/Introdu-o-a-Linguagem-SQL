# INTRODUÇÃO A LINGUAGEM SQL 📊

Nesse repositório você encontrará um NotebookLM para ajudá-lo a iniciar seus estudos na linguagem mais importante para quem quer seguir na área de dados, ou simplesmente, para quem quer aprender sobre ela. Com o  objetivo principal de facilitar o aprendizado nessa área, escolhi diversas fontes para formar os conhecimentos do modelo do NotebookLM.

## Mini Guia de Estudo 📖
### Resumo Estruturado
1. O que é um Banco de Dados?
Antes de entender a linguagem, entenda onde ela atua. Um banco de dados é uma coleção estruturada de dados.
A analogia do armário: Pense no banco de dados como um grande armário de escritório. Dentro dele, temos pastas (que são as Tabelas) e, dentro das pastas, temos as folhas de papel (que são os Registros ou linhas).
Tabelas e Colunas: Cada tabela é dividida em colunas (campos), como "Nome", "Idade" ou "E-mail", e cada linha representa uma entrada específica (ex: o cliente João).

2. Modelagem de Dados: Organizando a Casa
Antes de sair escrevendo código, você precisa pensar no modelo de dados: quais "entidades" do mundo real você quer guardar?
Chave Primária (PK): É o "CPF" do registro. Um valor único que identifica aquela linha e nunca se repete (ex: ID do Cliente).
Chave Estrangeira (FK): É como conectamos duas tabelas. Se um pedido pertence a um cliente, usamos o ID do cliente dentro da tabela de pedidos para criar esse vínculo.
Relacionamentos: As tabelas podem se relacionar de forma 1 para N (um cliente tem vários pedidos) ou N para N (vários produtos em vários pedidos), exigindo às vezes uma "tabela associativa" para ligá-los.

3. As Categorias de Comandos SQL
O SQL é organizado em subconjuntos, dependendo do que você quer fazer:
DDL (Definição): Comandos que criam ou alteram a estrutura (o "armário" e as "pastas"). Ex: CREATE, ALTER, DROP.
DML (Manipulação): Comandos para mexer nos dados dentro das pastas. Ex: INSERT (inserir), UPDATE (atualizar), DELETE (apagar).
DQL (Consulta): O comando mais usado para buscar informações: o famoso SELECT.

4. Primeiros Passos Práticos (Mão na Massa)
Criando sua primeira tabela
Para criar uma tabela, você define o nome e o tipo de dado de cada coluna (se é texto, número ou data).

CREATE TABLE produtos (

    id_produto INT PRIMARY KEY,
    nome VARCHAR(100) NOT NULL,
    preco DECIMAL(10,2)
);

Dica: VARCHAR é usado para textos de tamanho variável (como nomes), economizando espaço no servidor.
Consultando Dados (SELECT)
É aqui que a mágica acontece. Você pede ao banco o que quer ver.

SELECT * FROM produtos; — Traz tudo da tabela.

WHERE — Filtra os resultados (ex: apenas produtos com preço > 100).

ORDER BY — Organiza os dados em ordem crescente ou decrescente.

JOIN — Une dados de tabelas diferentes em um único resultado.

Manipulando os Dados
INSERT: Adiciona novos registros.
UPDATE: Altera registros existentes. Cuidado: sempre use o WHERE para não alterar a tabela inteira por acidente!

DELETE: Remove registros. Assim como no update, o WHERE é obrigatório para não apagar tudo!

5. Funções de Agregação (Resumos)
O SQL também sabe fazer contas para você:
COUNT(): Conta quantos registros existem.
SUM(): Soma valores.
AVG(): Calcula a média.
GROUP BY: Agrupa os resultados (ex: total de vendas por cidade).

## Fontes usadas:
https://www.youtube.com/watch?v=dpanYy8IrcU 
https://www.youtube.com/watch?v=KJ3LqI_X-Qo 
https://www.youtube.com/watch?v=BgUxpPKw2LI 
https://www.devmedia.com.br/guia/guia-completo-de-sql/38314 
https://cdn.bookey.app/files/pdf/book/pt/introdu%C3%A7ao-a-linguagem-sql.pdf 


Esse repositório é um projeto para o Bootcamp Accenture - Python para Ánalise e Automação de Dados.
