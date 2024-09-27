# Projeto de Análise da Empresa de Energia Solar Energia
<div style="display: flex; justify-content: space-between;"> <br>
<img width="1000" alt="netflix" src="https://github.com/MiguelTessele/Analise_Energia/blob/main/Capa.png">
  
# Sobre o Projeto:
- O objetivo primário deste projeto é desenvolver um painel que demonstre o cenário atual de vendas da empresa e o desempenho de seus produtos, o cliente solicitou a nós que fosse mantido o sigilo dos nomes do produtos, sua marca, então foi feita a mudança do logo da empresa e a nomenclatura dos produtos. Utilizamos uma base de dados que o cliente nos forneceu o acesso ao banco de dados deles através de acesso limitado onde após feita a extração dos dados foi exportado um arquivo em Excel. O primeiro painel fornecerá informações detalhadas sobre a visão geral da vendas, uma visão de linha temporal com o faturamento, faturamento por trimestre e qual foi a quantidade vendida dos produtos ao passar dos meses além de seu ticket médio. O segundo painel terá detalhes dos produtos que são comercializados pela empresa, identificar quais produtos estão sendo mais vendidos.
- Este painel será uma ferramenta essencial para as equipes da vendas, financeiro e para a própria diretoria. auxiliando nas tomadas de decisões estratégicas para aumentar o volume de vendas, identificar quais produtos estão sendo mais aceito pelo mercado. Através da análise detalhada dessas informações, espera-se identificar insights valiosos que contribuirão para novas vendas e criação de novos produtos.
<br />

# Etapas do Projeto (DataOps)
- Perguntas de negócio;
- Mapeamento dos dados;
- Prototipação;
- ETL (Extração, Transformação e Carregamento);
- Descobertas e insights;
- Sugestões de decisão.

<br />

# Perguntas de Negócio
Com o objetivo de fornecer um quadro geral dos insights a partir dos dados fornecidos, foi decidido que deveriam ser respondidas as seguintes perguntas: 
- Qual foi o trimestre que ocorreu faturamento?
- Qual é o Ticket Médio?
- Total do faturamento?
- Qual mês obtivemos mais vendas?
- Qual produto está nos dando mais retorno?

  Respondidas essas perguntas, as respostas fornecerão um quadro geral do cenário atual e do comportamento das vendas, permitindo uma compreensão mais aprofundada de suas necessidades.


<br />

# Mapeamento dos Dados
- Os dados foram extraidos do banco de dados para um arquivo xlsx e estruturados no Power Query.
 <img width="1000" alt="Imagem dados" src="https://github.com/MiguelTessele/Analise_Energia/blob/main/Base_Original.png">

 
<br />
 


# Prototipação
Com base no entendimento do problema, foram desenvolvidas as telas de prototipação para o desenvolvimento dos dashboards. Essas telas prototipadas servirão como guia para a construção dos dashboards finais, garantindo que todas as necessidades e objetivos identificados sejam atendidos.A ferramenta utilizado foi o Figma, permitindo visualizar uma prévia de como ficará a entrega final. Foi utilizado o Adobe Color para extrair o número HEX de cada cor.

#### Protótipo página 1

 <img width="1000" alt="Imagem dados" src="https://github.com/MiguelTessele/Analise_Energia/blob/main/Prot%C3%B3tipo%201.png">

#### Protótipo página 2

<img width="1000" alt="Imagem dados" src="https://github.com/MiguelTessele/Analise_Energia/blob/main/Prot%C3%B3tipo%202.png">



# ETL (Extração, Transformação e Carregamento)
### Preparação dos dados
- 	Extração da base feita para o Power Query;
-   Limpeza de dados inconsistentes;
-   Coluna com valores "null" foram excluidas pois não tinham relevância;
-   Mudança dos tipos de coluna: A coluna de "Data" estava com tipo de coluna Texto/ Número Inteiro, foi ajustado para o tipo correto Data, a coluna "Produto" foi feita as mesmas alterações da coluna Data. A coluna "Quantidade Vendida" foi ajustada para tipo de número inteiro e a coluna "Faturamento" foi ajustada para Número Decimal Fixo;
-   Arredondamento das casas decimais (2 casas);
-   Carregamento dos dados limpos para o Power BI.

 <img width="1000" alt="Imagem dados" src="https://github.com/MiguelTessele/Analise_Energia/blob/main/Base_Formatada.png">
 
 
<br />
  
<br />
 
 
  
# Dashboard Interativo
Com os dados devidamente processados, começamos a elaboração de visualizações com dados estatísticos pertinentes, que servirão como base para responder às questões propostas inicialmente. Foi necessário desenvolver algumas medidas utilizando fórmulas DAX para melhor analisar os dados e extrair insights significativos.

- [Clique aqui para visualizar o dashboard de maneira interativa](https://app.powerbi.com/reportEmbed?reportId=4d257bbc-ca04-41c5-a2f6-3d46d8d407bd&autoAuth=true&ctid=f5a6833e-3f93-41ac-8092-ee06a0910899)

<br />
 
![DASHBOARD_1](https://github.com/MiguelTessele/Analise_Energia/blob/main/DASHBOARD_1.png)

![DASHBOARD_2](https://github.com/MiguelTessele/Analise_Energia/blob/main/DASHBOARD_2.png)



<br />
<br />


# Descobertas e Insights
<img width="1000" src="https://github.com/MiguelTessele/Analise_Energia/blob/main/Insights.png">


Após a finalização do dashboard e a realização de uma análise minuciosa do material, foram observados os seguintes insights:
- O produto E lidera com o maior total de vendas. Pode ser interessante fazer uma pesquisa para entender qual a sua aceitação no mercado, o que diferencia ele de outros produtos.
- O mês que obtivemos vendas maior foi em maio, seguido por julho e setembro. É interessante analisarmos esses meses e verificar se ocorreu algum desconto nos produtos, procura mais do 
mercado ou foi devido as fortes chuvas que ocorreram no Rio Grande do Sul causando as enchentes e destruindo os produtos fazendo com que fossem adquiridos novamente.
-  Verificar como o faturamento varia ao longo do tempo (mensal, trimestral, anual) para identificar períodos de alta e baixa.
- O ticket médio por transação é relativamente baixo. A empresa pode estar vendendo produtos de baixo valor unitário em grandes quantidades.

 
 <br />

  
 
 # Recomendações ao tomador de decisão

 <img width="1000" alt="Imagem dados" src="https://github.com/MiguelTessele/Analise_Energia/blob/main/Recomenda%C3%A7%C3%B5es.png">
 
Com base nos insights alcançados, algumas alternativas foram propostas aos dirigentes para que a empresa possa aprimorar seus resultados:
- Identificar as informações do produto E, identificar quais as condições de ofertas para podermos replicar as ofertas em alguns outros produtos ou até mesmo criar um produto novo com tecnologia mais avançada que o produto E.
- Verificar o histórico dos anos anteriores para verificar se é uma sazonalidade, olhar para as ofertas comparadas aos outros meses, caso não seja nenhum desses fatores devemos observar se foi devido a enchente fazendo um estudo de qual regiões ocorreu a aquisição dos produtos.

<br />

