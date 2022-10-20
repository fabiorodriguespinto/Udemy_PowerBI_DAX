Udemy_PowerBI_DAX


Curso Udemy

Curso de Power BI + Dax + Projetos na prática.

Sobre este curso
Aprenda Microsoft Power BI - Transforme seus dados 
em informações Visuais usando as melhores Práticas.



Seção 1: Introdução - 3 aulas - 9min

Aula_01: Apresentação Instrutor

Aula_02: Resumo do Curso

Aula_03: Boas Vindas, Dicas e Material para download



Seção 2: Instalando a BI - 3 aulas - 12min

Aula_01: Instalação do Power BI

Aula_02: Overview do Power BI

Aula_03: Configurações Básicas



Seção 3: Introdução a BI - 9 aulas - 58min

Aula_01: O que é BI


Aspectos teoricos

Definições:


- Power Bi é uma ferramenta de apoio a tomada de decisão, e ela busca gestão de performance e oportunidades para o negócio e atraves dessas oportunidades, alcançar ou aumentar o lucro;

- É um conjunto de processos e metodologias, implementadas por meio de ferramentas de software , para obter informação e conhecimento útil para a tomada de decisão.

- Segundo BARBIERI, 2001:

"Utilizando de várias fontes de informação para definiçaõ de estratégias de competitividade nos negócios"


- Segundo LOSCHIN, 2003:

"Processos, tecnologias e ferramentas para tornar dados em informaçãoes, informações em conhecimento e conhecimento me planos que guiam ações em negócios lucrativos"


Qual o foco?

Prover acesso a informação;
Apresentar a informação;
Objetivos estratégicos;
Oportunidades de negócio.

Faz uso

Armazem de dados - DATA WAREHOUSE;
Ferramentas analíticas e recursos gráficos - OLAP;
Identificação automatizada de Padrões e relacionamentos.


Há diversas ferramentas de BI

PowerBI;
Tableau;
Qlik;
ThoughtSpot;
Diversas outras.



Aula_02: Ciclo de informação

O ciclo da informação segue o esquema abaixo: 

Dados
- Planilhas
- Bancos de dados
- Internet

Informação
- Gráficos
- Relatórios
- Infográficos
- Dashboards

Conhecimento
- Conhecer
- Compreender
- Fatos


Tudo que se mede pode ser representado por um gráfico.

Um exemplo simples:


Dados:

Contas			-		Valor
Luz						75
Água			-		50
Supermercado	-		500	
Combustível		-		65
Lazer			-		200

Salário			-		1000	

Informação:

Descrição		-		Valor
Total a Pagar	-		 890
Total a Receber	-		1000
Saldo			-		110

Conhecimento:


Interpretação da informãção, na forma de um gráfico, que exiba faixas de consumo, indicando uma severidade nos valores gastos e recebidos.

No exemplo acima, os dados são os valores recebidos e gastos, segundo os dados, a informação gerada foram os totais a pagar e a receber e uma terceira informação, totalmente nova, que é o saldo.

O conhecimento se dá pela interpretação das informaçãoes para gerar um dashboard onde é possível verificar os gastos e o saldo remanescente, bem como uma tomada de decição sobre o que fazer com o saldo remanescente.


Aula_03: O que é ETL


Extract, Transform and Load

O ETL visa trabalhar com toda a parte de extração de dados de fontes externas, transformação para atender às necessidades de negócios e carga dos dados dentro do Data Warehouse.


Requisitos do ETL

Requisitos do negócio:
É preciso definir claramente quais são os requistos do negócio.

Viabilidade dos dados:
É preciso realizar uma analise de viabilidade dos dados, se os dados existem e são acessiveis.

Latencia dos dados:
Tempo máximo permitido para disponibilização dos dados através do sistema de BI, é o tempo da carga no PowerBI, pode ser tmb o tempo de consulta ao BD.

Politicas de Compliance e Segurança:
Quem vai ter acesso a informação, se pode ter acesso a esta informação, é preciso haver segurança para que as pessoas certas tenham acesso a informação e recebam a informação no tempo certo onde ainda são relevantes.



Aula_04: O que é DW e DM

O Data Warehouse é onde os dados são guardados.

Data Mart são banco de dados espeficicos para cada assunto, exemplo, os dados para o departamento de marketing.



Aula_05: Tabelas Fato e Dimensão


Em um Data Warehouse, uma tabela que armazena os valores detalhados de medidas, ou fatos, é denominada 
de tabela fatos.

Uma tabela de dimensão contém o nome especifico de cada membro da dimensão.


Aula_06: O que é Star Schema e Snow Flake

Star Schema - modelo estrela

O esquema estreja é composto no centro por uma tabela fato, rodeada por tabelas de dimensão.

Snow Flake - modelo floco de neve


Aula_07: O que é OLTP e OLAP


OLTP - On line transaction Processing
OLAP - On line analitical Processing


Aula_08: Sistemas operacionais e Analitícos


OLTP é um sistema operacional
OLAP é um sistema analitico.


Aula_09: Passos para Modelagem Dimensional

Passo 1 O que estamos avaliando?
Passo 2 Como serão avaliados ou analisados?
Passo 3 Qual o nivel mais baixo de detalhes das informações?
Passo 4 Como se espera agrupar ou sumarizar as informações?


Momento descontração:


<div id="header" align="center">
  <img src="https://media.giphy.com/media/8dYmJ6Buo3lYY/giphy.gif" width="100"/>
</div>



Seção 4: Hands on! Importando dados - 16 aulas - 1h 53min


Aula_01: Apresentação do Modelo

Apresentação da base de dados em excel que será utlizada nesta seção.


Aula_02: Importando dados do Excel

Importando dados do Excel, pasta e CSV.

Para esta aula, será realizada a importação de uma tabela da base de dados em excel.

Para isto, abra o PowerBI, clique em "Obter dados" ou ao abrir o ícone, na linha "Mais", na janela aberta, há os tipos de dados nas linhas a esquerda e as opções para cada linha da esquerda na seção a direita.

Para iniciar, selecione o tipo "Arquivo" e na coluna da direita, "Pasta de Trabalho do Excel", clique no botão conectar, nevegue até o diretório do arquivo excel e selecione o arquivo Base_vendas.

Na janela aberta, selecione a tabela dimensão D_Clientes. Ao clicar a tabela é exibida a direita, clique no botão "Transformar Dados".

Na nova janela aberta, temos a exibição da tabela e o painel a direita, onde é possível ver "AS ETAPAS APLICADAS"  que são o histórico das ações ou alterações realizadas na tabela.

Ajustando a tabela:

Por padrão o PowerBI identificou o campos das primeiras linhas como o nome dos campos e atribui o tipo de dado conforme o preenchimento.

Para não gastar processamento com campos que não são numéricos e que não serão utilizados em analises, vamos alterar o tipo de alguns campos.

O tipo fica no início do cabeçalho de cada coluna, para modificar, clique sobre o tipo e escolha o tipo desejado. No caso vou modificar o tipo da coluna Cod_Cliente de númerico para texto. Na janela que abri clique no botão "Adcionar nova etapa", vou repetir para a coluna Cod_uf, após os ajustes, clique no ícone "Fechar e Aplicar"


Aula_03: Importando dados do Excel

Importar todos as tabelas da Base_vendas, exceto a D_Clientes já importada na aula anterior sem realizar nenhuma pré edição.

Editar os campos e alterar os tipos onde não for necessário o tipo de dados numérico. Percorrer cada tabela e verificar os campos de cada tabela.

Abrir o Power Query, e editar os itens das tabelas de para que não haja tabelas com tipos errados.

Ao iníciar as transformações, começamos a realizar o ETL.


Aula_04:
Aula_05:
Aula_06:
Aula_07:
Aula_08:
Aula_09:
Aula_10:
Aula_11:
Aula_12:
Aula_13:
Aula_14:
Aula_15:
Aula_16:
