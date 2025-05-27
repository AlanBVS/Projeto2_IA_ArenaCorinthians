Projeto 2 - Inteligência Artificial
Sobre
Este projeto cria uma pipeline de aprendizado de máquina para prever resultados de partidas na Arena Corinthians, usando o dataset do Kaggle. O notebook, executado no Google Colab, inclui análise de dados, transformações, treinamento de um modelo Random Forest, avaliação e predição.
Observação: O projeto analisa 321 partidas, codifica times visitantes, remove dados faltantes, divide o dataset em treino, validação e teste, e prevê se o Corinthians vence, empata ou perde, com acurácia de cerca de 60-70%.
Requisitos

Ambiente: Google Colab (já inclui bibliotecas).
Bibliotecas: pandas, numpy, scikit-learn, matplotlib, seaborn.
Dataset: A - Jogos.csv (Arena Corinthians).
Opcional: kaggle.json para baixar via API.

Como Reproduzir

Abrir o Notebook:

Acesse: https://colab.research.google.com/drive/1_ep-6UFDi-o44fCPj55p9JkHs10rRRzR?usp=sharing.


Obter o Dataset:

Via API do Kaggle:
Baixe kaggle.json em Kaggle > Settings > API.
No Colab, execute:!pip install kaggle
from google.colab import files
files.upload()  # Upload kaggle.json
!mkdir -p ~/.kaggle
!cp kaggle.json ~/.kaggle/
!chmod 600 ~/.kaggle/kaggle.json
!kaggle datasets download -d danilosoares/arena-corinthians --force
!unzip arena-corinthians.zip




Upload Manual:
Baixe A - Jogos.csv em Kaggle.
No Colab, clique na pasta (📁) e faça upload do arquivo.




Executar:

Clique em Runtime > Run all ou execute célula por célula (Shift + Enter).
Saídas incluem estatísticas, gráfico, acurácia, matriz de confusão e predição.



Vídeo de Apresentação

Acesse:  https://youtu.be/R6EPhJaAvKI?si=ZV8PXSQyT1aObMOV

Dataset

Fonte: Arena Corinthians
Licença: Copyright dos autores
Conteúdo: 321 partidas, com gols, time visitante, público, etc.

Autor

Nome: Alan Bruno


