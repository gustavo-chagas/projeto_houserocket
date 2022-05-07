# Projeto de Insights
Análise de dados públicos para geração de insights utilizando o Jupyter Notebook

## Contexto do projeto
A empresa House Rocket Company é uma empresa de compra e venda de casas, o CEO da empresa solicitou a mim que fosse feito uma análise de dados com base em um dataset de modo a ajudar o time de negócio com as oportunidades de compra e venda por meio da geração de insights.

## Premissas do negócio
- Não podem existir casas com número de banheiros ou quartos iguais a 0, esses casos podem ser interpretados como imóveis comerciais ou apenas erro humano.
- Casas com quantidades de quartos ou banheiros acima de 4 vezes a quantidade do primeiro quartil serão consideradas como outliers ou erros humanos e removidas do dataset.
- A sazonalidade pode influenciar nos preços de imóveis, devido ao clima, neve, período escolar e dificuldades na mudança.(https://www.investopedia.com/articles/investing/010717/seasons-impact-real-estate-more-you-think.asp)
- Nos Estados Unidos, o total de banheiros de uma casa pode não ser um número inteiro, visto que para um banheiro ser considerado como completo, ele precisa ter 4 elementos. Caso haja menos que 4, são utilizadas frações, como 3/4, 2/4 (ou 1/2) e 1/4. (https://www.thespruce.com/types-of-bathrooms-4800093)

## Planejamento da solução
- Sabendo que a localização é um grande fator na precificação de uma casa, pode-se buscar oportunidades com base em indicadores de localização.
- Também é possível buscar oportunidades por meio de reformas nas casas compradas, seja apenas renovando a estrutura de casas velhas como também adicionando cômodos.
- Usar a sazonalidade à favor na hora de vender para conseguir melhores preços.

## Insights do negócio

### Existem casas em boas condições com valor abaixo de 50% do valor da mediana da área. 
VERDADEIRO. A porcentagem máxima de diferença chega à 67,84%.
### A diferença de preço mediano entre casas com 1 e 2 quartos é maior do que a diferença entre as outras quantidades de quartos. 
FALSO. A maior diferença de preço fica entre casas com 3 e 4 quartos.
### Imóveis construídos até 1950 e que foram reformados tem preços 20% maiores do que os que não foram reformados, em média. 
FALSO. A diferença fica em torno de 40%.
### Imóveis com porão são 20% mais caros que imóveis sem porão. 
VERDADEIRO. A diferença realmente fica em torno de 20%.
### É possível ter diferença de preços médios de imóveis de 10% entre meses devido à sazonalidade. 
VERDADEIRO. Entre os meses de fevereiro e abril de 2015 a diferença ficou em torno de 10%.

## Resultados financeiros
Ao final do notebook, foi construída uma lista com a recomendação de compra de 5 casas. Todas foram anunciadas em Novembro de 2014 (que é o segundo melhor mês para compras), não possuem porão, possuem 3 quartos cada e boas condições, além disso, foram construídas antes de 1950 e não foram reformadas. Todas da lista também estão abaixo do valor mediano de seu respectivo zipcode, as tornando opções atrativas para a compra.

Caso a empresa deseje comprar todas as casas e revender nos meses de Abril ou Maio ao preço da mediana de zipcode, seria possível realizar um lucro de aproximadamente 216.355 dólares. Esse lucro ainda poderia ser aumentado, visto que essas casas possuem alto potencial de aumento de valor por meio de reformas, seja por meio da criação de um porão ou adição de um quarto. Segundo pesquisa, a adição de um porão ou quarto novo gira em torno de 50 a 60 mil dólares, em média, na cidade de Seattle, levando em conta esses custos e adicionando um valor de 30% sobre as casas na venda, o lucro líquido estimado subiria para 276.093 dólares.

## Conclusão
É possível concluir que no dado dataset existem boas oportunidades para a compra de casas, tanto para revenda simples como também para a agregação de valor por meio de reformas, de maneira que o time de negócios poderia tomar uma decisão melhor embasada sobre o negócio. Como o objetivo estabelecido do projeto é gerar insights e recomendar uma lista de recomendação de compra para ajudar a equipe de negócios, pode-se concluir que o projeto alcançou seu objetivo.

## Próximos passos
Aprender sobre algoritmos de Machine Learning para aplicar no dataset de maneira a obter as diferenças entre os valores previstos pelo algoritmo e os valores dos anúncios.
