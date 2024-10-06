# Pasta dedicada a base de dados do modelo

# Sobre o Dataset

A base de dados que escolhemos trata das músicas mais reproduzidas no Spotify, incluindo detalhes como título da música, artista, ano de lançamento e demais métricas.

## Descrição do Dataset

A base de dados trata-se das músicas mais transmitidas no Spotify dentro de um intervalo de tempo definido, tornando evidente tendências musicais e preferências dos usuários. Escolhemos essa base de dados pois a achamos útil para análises estatísticas, estudos de tendências, machine learning e outras aplicações relacionadas ao campo da IASSSS.

## Atributos do Dataset

- **Position**: Posição da música no ranking das mais reproduzidas.
- **Track Name**: Nome da música.
- **Artist**: Nome do artista ou banda.
- **Streams**: Número de reproduções da música.
- **URL**: Link para a música no Spotify.
- **Album**: Nome do álbum ao qual a música pertence.
- **Release Date**: Data de lançamento da música ou do álbum.
- **Length (ms)**: Duração da música em milissegundos.
- **Popularity**: Índice de popularidade no Spotify.
- **Danceability**: Medida de quão dançável é a música.
- **Energy**: Nível de energia da música.
- **Key**: Chave musical (nota) da música.
- **Loudness (dB)**: Volume médio da música em decibéis.
- **Mode**: Modalidade da música (maior ou menor).
- **Speechiness**: Presença de palavras faladas na música.
- **Acousticness**: Medida de quão acústica é a música.
- **Instrumentalness**: Probabilidade de a música ser instrumental.
- **Liveness**: Probabilidade de a música ter sido gravada ao vivo.
- **Valence**: Positividade musical transmitida pela música.
- **Tempo**: Velocidade da música em batidas por minuto (BPM).

## Fonte

Os dados foram obtidos do Kaggle: [Spotify Most Streamed Songs Dataset](https://www.kaggle.com/datasets/abdulszz/spotify-most-streamed-songs)



## Tratamento dos Dados e Uso no Modelo

Para preparar o dataset para uso em nosso modelo de redes neurais, seguimos os seguintes passos:

### 1. Exploração e Entendimento dos Dados

- **Análise Exploratória**: Iniciamos com uma análise exploratória para entender a distribuição das variáveis, identificar possíveis inconsistências e detectar valores ausentes. Fizemos também análise das variáveis que julgamos mais interessantes para utilizar no modelo.

### 2. Limpeza dos Dados

- **Tratamento de Valores Ausentes**: Verificamos a presença de valores nulos e optamos por remover registros incompletos para manter a qualidade dos dados.
- **Remoção de Duplicatas**: Eliminamos registros duplicados para evitar vieses nos resultados do modelo.
- **Correção de Tipos de Dados**: Ajustamos tipos de dados quando necessário, garantindo que todas as colunas estivessem no formato adequado para análise.

### 3. Seleção de Características

- **Features Selecionadas**: Escolhemos um conjunto de características numéricas que influenciam a popularidade das músicas, como:
  - `danceability` - (quão dançável é a música)
  - `energy`
  - `loudness`
  - `speechiness`
  - `acousticness`
  - `instrumentalness`
  - `liveness` - (ânimo da música)
  
- **Variável Alvo**: Decidimos utilizar a coluna `popularity` como variável alvo, transformando-a em uma classe binária para classificação:
  - **Popular**: Músicas com popularidade acima de um determinado limiar.
  - **Não Popular**: Músicas com popularidade abaixo desse limiar.

### 4. Codificação de Variáveis Categóricas

- **One-Hot Encoding**: Aplicamos a codificação one-hot em variáveis categóricas, como `key` e `mode`, para converter esses dados em um formato numérico adequado para o modelo. //////////


### 5. Normalização e Escalonamento

- **Escalonamento**: Utilizamos o `MinMaxScaler` para normalizar as features numéricas, escalando os valores para um intervalo entre 0 e 1.
- **Justificativa**: A normalização é importante para que nenhuma característica domine as outras devido à escala, melhorando o desempenho e a velocidade de convergência do modelo.

### 6. Divisão dos Dados

- **Conjunto de Treinamento**: 70% dos dados foram utilizados para treinar o modelo.
- **Conjunto de Validação**: 15% dos dados serviram para validar e ajustar os hiperparâmetros.
- **Conjunto de Teste**: 15% dos dados foram reservados para avaliar a performance final do modelo.

### 7. Decisão de Uso no Modelo

- **Escolha do Problema**: Optamos por um problema de **classificação binária** para prever se uma música será popular ou não, com base em suas características.
- **Motivação**: A predição da popularidade pode fornecer insights valiosos para artistas, produtores e a indústria musical em geral.


### 10. Avaliação dos Resultados

- **Desempenho do Modelo**:
  - A melhor configuração alcançou uma acurácia de **X%** no conjunto de teste.
- **Conclusões**:
  - asdasd