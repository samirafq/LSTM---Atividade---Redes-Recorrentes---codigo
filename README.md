# Classificação de Sentimentos com LSTM

## Descrição
Implementação de uma rede neural LSTM utilizando TensorFlow/Keras para classificação de sentimentos em avaliações de filmes do dataset IMDB.

O modelo identifica se uma avaliação possui sentimento positivo ou negativo.

## Estrutura do modelo
- **Embedding:** transforma as palavras em vetores numéricos.
- **LSTM:** processa as sequências e armazena informações importantes.
- **Dense:** realiza a classificação final utilizando a função Sigmoid.

## Treinamento
O modelo foi treinado durante 3 épocas, utilizando:
- Dataset: IMDB.
- Vocabulário: 10.000 palavras.
- Tamanho das sequências: 200.
- Batch size: 64.
- Otimizador: Adam.

## Resultados

| Época | Acurácia de treinamento | Acurácia de validação |
|---|---:|---:|
| 1 | 78,96% | 86,80% |
| 2 | 90,23% | 87,24% |
| 3 | 93,57% | 87,40% |

**Acurácia final no teste: 86,04%.**

## Conclusão
O modelo conseguiu classificar os sentimentos das avaliações com 86,04% de acurácia nos dados de teste, demonstrando o funcionamento da rede LSTM na identificação de sentimentos em textos.
