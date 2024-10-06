# UC: Inteligência Artficial
## Atividade 4 – Redes Neurais e Aprendizado Supervisionado

### Professor: Otaviano Silvério de Souza.

### Alunos:
### - Ian Matsuhara Ferraz (RA: 1242021408)
### - Diego Diniz Amaral de Sá (RA: 12119820)

# O Conceito de Aprendizado Supervisionado

O aprendizado supervisionado é uma abordagem na qual o modelo usado é treinado em conjunto com dados rotulados. Significa que cada entrada vem acompanhada de um rótulo ou resultado esperado por ele. O objetivo é aprender e mapear as entradas de modo que, ao ser apresentado novos dados – esses, sem rótulo – o modelo seja capaz de prever os resultados – as saídas – que esses dados irão resultar em de maneira precisa.

# Comparação e Diferenças: Aprendizado Supervisionado e Não Supervisionado

O aprendizado não supervisionado, como seu próprio nome indica, faz o oposto do que o supervisionado faz em seu treinamento. Os dados que são entregues durante o não supervisionado não possuem rótulos e nem saídas esperadas, o objetivo dele é identificar padrões ou estruturas nos dados, sem ter conhecimento da resposta correta de antemão.
O aprendizado supervisionado, como dito anteriormente, busca um mapeamento específico de entradas para as suas saídas, já o não supervisionado busca entender a estrutura dos dados para assim agrupá-los como necessário. 

# Comparação e Diferenças: Aprendizado Supervisionado e por Reforço
O aprendizado por reforço faz com o que o agente interaja com o ambiente em que se encontra e aprenda uma política para maximizar recompensas cumulativas. Ele não recebe exemplos explícitos de quais ações deve tomar, mas sim um feedback que pode ser positivo ou negativo com nas ações que escolheu.
Sua diferença principal quando comparado com o aprendizado supervisionado é que o supervisionado requer um conjunto de rótulos para cada entrada, enquanto o por reforço envolve tomar decisões sequenciais em prol de maximizar as recompensas em seu cenário interativo.


# Rede Neural Artificial 
Uma rede neural artificial é um modelo computacional inspirado na estrutura do cérebro humano, composto por múltiplos "neurônios" interconectados - também conhecidos como Perceptrons -. Esses neurônios são organizados em camadas que processam informações de maneira sequencial ou paralela. A estrutura básica de uma rede neural pode ser dividida em três tipos principais de camadas: A camada de entrada, a camada oculta e a camada de saída. Cada neurônio realiza operações matemáticas, como somar os valores recebidos e aplicar uma função de ativação, antes de propagar o resultado para os neurônios das camadas seguintes.

# Camada de Entrada (Input Layer)
Essa camada é a responsável por receber os dados de entrada para a rede. Cada neurônio nela representa uma característica ou atributo do dado de entrada. Os neurônios dessa camada apenas distribuem os valores dos dados para a próxima camada, eles não realizam nenhum cálculo.

# Camada Oculta (Hidden Layer)
Essas camadas realizam a maior parte do processamento e da extração de padrões dos dados. Elas podem variar em número e quantidade de neurônios. Cada neurônio na camada oculta aplica uma função de ativação. O objetivo das camadas ocultas é aprender representações cada vez mais complexas dos dados de entrada à medida que a informação é passada por cada uma delas.

# Camada de Saída (Output Layer)
Essa camada produz a resposta final da rede. O número de neurônios dela depende do tipo de problema que a rede está resolvendo. Cada neurônio na camada de saída, assim como nas camadas ocultas, aplica uma função de ativação, dependendo do problema.
