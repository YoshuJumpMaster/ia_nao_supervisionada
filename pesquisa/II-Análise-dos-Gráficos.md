# II  - Análise Detalhada dos Resultados

![Matriz de Confusão](https://i.imgur.com/78Ku4H2.png)

Acima estão os resultados da precisão do modelo ao tentar classificar corretamente os dados das músicas que recebeu entre “Popular” e “Não Popular”.  As linhas representam os rótulos verdadeiros (o valor real dos dados informados), enquanto as colunas representam os rótulos preditos pelo modelo.  

- Verdadeiro Negativo (46): O número de músicas que eram realmente não populares e foram corretamente classificadas como não populares pelo modelo. Levando em conta o resultado e o gráfico usado acima, o modelo foi capaz de identificar com sucesso a maioria das músicas que não são populares.
- Falso Positivo (26): O número de músicas que eram não populares, mas foram incorretamente classificadas como populares. Isso reflete o problema de falsos alarmes, onde o modelo erroneamente atribui popularidade a músicas que não são, na verdade, populares.
- Falso Negativo (34): O número de músicas que eram populares, mas foram classificadas como não populares. Esse erro é problemático, pois significa que o modelo está falhando em reconhecer algumas músicas que deveriam ser identificadas como populares.
- Verdadeiro Positivo (37): O número de músicas que eram realmente populares e foram corretamente classificadas como populares. Indica que o modelo tem alguma habilidade para reconhecer músicas que são populares.

A alta quantidade de falsos negativos (34) e falsos positivos (26) indica que o modelo está tendo problemas em classificar músicas populares corretamente, e também está se confundindo ao achar que algumas músicas não populares são populares.

Abaixo temos um gráfico mostrando a perda e a precisão do modelo durante o treinamento:

![Perda e Precisão durante o Treinamento](https://i.imgur.com/jcCrWt2.png)

O gráfico à esquerda mostra a perda do modelo ao longo das épocas para os conjuntos de treino e validação. O eixo X representa o número de épocas, e o eixo Y representa o valor de perda.

A linha azul mostra a perda no conjunto de treinamento, é possível notar uma oscilação considerável, sugerindo que o modelo está flutuando bastante durante o aprendizado. Isso pode ser um indício de um aprendizado instável ou de um modelo que está tendo dificuldade para minimizar a função de perda de forma consistente.
Já a linha laranja indica a perda no conjunto de validação. A perda de validação é consistentemente mais alta que a perda de treinamento, indicando que o modelo está se ajustando melhor aos dados de treino, mas não está generalizando bem para dados que não foram vistos anteriormente. 
A perda média para treinamento e validação permanece alta (em torno de 0,675 a 0,690, como mostrado no gráfico), sugerindo que o modelo está com um desempenho inferior, provavelmente devido à dificuldade de separação entre classes.
