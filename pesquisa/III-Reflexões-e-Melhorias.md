# III  - Reflexões sobre o Impacto das Alterações e Possíveis Melhorias

Os gráficos indicam que o modelo está enfrentando problemas de instabilidade no treinamento, impactando negativamente a sua precisão e a sua capacidade de generalização.

A diferença significativa entre a perda e a precisão nos conjuntos de treino e validação sugere que o modelo está ajustado demais aos dados de treinamento e não consegue capturar padrões robustos que se traduzam para novos dados. 
As oscilações na curva de perda e precisão indicam uma taxa de aprendizado inadequada, que poderia ser ajustada para estabilizar o processo de otimização.

Após fazermos uma investigação, chegamos na conclusão de algumas melhorias que podem ser feitas: 

- Aumento de Dados: Adicionar mais exemplos ao conjunto de dados pode ajudar o modelo a aprender padrões mais diversos.
- Cross-Validation: Implementar uma validação cruzada mais rigorosa pode fornecer uma visão mais robusta do desempenho e evitar dependência dos dados de treino.

Considerando que estamos lidando com um conceito abstrato como “música”, especialmente ao tentar desenvolver um cálculo para prever se uma música será popular ou não, é essencial reconhecer as limitações inerentes das abordagens baseadas em inteligência artificial para esse tipo de tarefa. 
É importante admitir que atingir um nível de precisão de 100% neste contexto é irrealista. A capacidade de quantificar atributos que determinam a popularidade de uma música está além das possibilidades atuais, sendo que o melhor resultado que conseguimos obter é uma aproximação, utilizando a transformação de certas características musicais em valores numéricos. Ainda assim, esse processo permanece subjetivo e depende de decisões arbitrárias no modelo.
