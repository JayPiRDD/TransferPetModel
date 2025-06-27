# Projeto Cats vs Dogs com Transfer Learning - Bootcamp DIO

## Descrição

Este projeto tem como objetivo criar um classificador de imagens que distingue gatos e cachorros utilizando Transfer Learning com MobileNetV2 pré-treinado no ImageNet. É um projeto didático feito durante o Bootcamp de Machine Learning da plataforma DIO, ideal para iniciantes.

## Estrutura do Projeto

1. **Importação das bibliotecas:** TensorFlow, TensorFlow Datasets e Matplotlib para manipulação, modelagem e visualização.
2. **Carregamento e preparação dos dados:**
   - Dataset Cats vs Dogs do TensorFlow Datasets.
   - Divisão em conjuntos de treino (80%) e validação (20%).
   - Função de pré-processamento para redimensionar imagens para 160x160 e normalizar pixels.
3. **Visualização dos dados:**
   - Exibição de imagens com seus rótulos para familiarização com o dataset.
4. **Configuração do modelo:**
   - Uso do MobileNetV2 pré-treinado (congelado).
   - Adição de camadas finais para classificação binária.
5. **Treinamento do modelo:**
   - Compilação com otimizador Adam e função de perda binary_crossentropy.
   - Treinamento por 5 épocas com monitoramento da acurácia e perda.
6. **Avaliação do modelo:**
   - Avaliação no conjunto de validação para medir desempenho.
   - Visualização das previsões do modelo em imagens reais.
7. **Visualização final:**
   - Apresentação de 10 imagens (5 gatos e 5 cachorros) do conjunto de validação para análise visual.

## Como executar

1. Instale as dependências:

```bash
pip install tensorflow tensorflow-datasets matplotlib
