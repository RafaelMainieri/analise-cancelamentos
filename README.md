# Análise de Cancelamento
O projeto foi criado com o intuito de analisar uma base de dados de clientes de uma empresa, onde se faz todo o tratamento dessas informações e é retornado em formato de gráfico (para mais fácil entendimento) as causas dos cancelamentos. Ao final é mostrado o impacto positivo para a empresa caso esses cancelamentos fossem resolvidos, que, no exemplo utilizado seria uma diminuição de 38%.
## Funcionamento
- Importar a biblioteca pandas e ler a base de dados com **tabela = pd.read_csv(‘arquivo’)*;
- Retirar as colunas inúteis para a análise com tabela.drop(columns=x);
- Visualizar as informações da base de dados com tabela.info() e retirar linhas que contenham erros de preenchimento com tabela.dropna();
- Visualizar a quantidade e porcentagem dos cancelamentos para melhor análise;
- Importar a biblioteca plotly e analisar as causas do cancelamento de acordo com o gráfico mostrado com gráfico = px.histogram(tabela, x=coluna, color=’cancelou’) e gráfico.show();
- Calcular o impacto desses cancelamentos para a empresa caso fossem resolvidos. Um dos exemplos dessa análise seria a duração do contrato, que seria: tabela = tabela[tabela[‘duracao_contrato’]!=’Monthly’], onde de acordo com a condição estabelecida, todos os clientes com o contrato mensal seriam retirados da análise.
## Adaptações
- Informar a base de dados correta a ser analisa na variável “tabela”. (bloco 2, linha 3);
- Analisar a base de dados e apagar as colunas inúteis. (bloco 2, linha 7);
- Se necessário, modificar o nome da coluna onde é informado se o cliente cancelou. (bloco 4, linha 2);
- Se necessário, modificar a str da “color” no código grafico = px.histogram(tabela, x=coluna, color=’cancelou’) para o nome da coluna informada na sua base de dados. (bloco 5, linha 4);
- Modificar as condições, analises e colunas na base de dados. (bloco 6);
## Observações
A análise pode ser feita de acordo com as preferências da empresa, onde pode-se analisar cada item de forma individual, assim obtendo resultados melhores e personalizados. <br>
Ao final do código dei algumas sugestões rápidas para a solução dos problemas de cancelamento analisados.

 
