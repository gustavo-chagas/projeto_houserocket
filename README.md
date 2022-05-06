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
