# Projeto Final
Classificação de imagens de raio-X divididas entre as classes: covid e normal.

## Equipe 

Alan Araújo Oliveira 

## Descrição do descritor implementado


Para a extração de características das imagens do projeto, foi utilizado o descritor LBP (Local Binary Pattern).
O descritor LBP é um descritor de textura em imagens que compara os valores de intensidade dos pixels vizinhos com o valor do pixel central. O mesmo gera padrões binários locais para cada pixel da imagem, representando a textura da imagem.

## Repositório do Projeto

O código fonte e demais arquivos relacionados ao projeto estão disponíveis no repositório [projetoFinalClassificador](https://github.com/lanoliveira/projetoFinalClassificador).

## Vídeo de Apresentação
[*Apresentação do projeto.*](https://drive.google.com/file/d/1wIbzf2vNau3g9SIb6bdsEDNqn2sTnc2L/view?usp=sharing)

## Dataset

O dataset utilizado foi o [COVID-19 & Normal Posteroanterior(PA) X-rays](https://www.kaggle.com/tarandeep97/covid19-normal-posteroanteriorpa-xrays), o mesmo é composto por 280 imagens de raios-X de tórax e estão dividos em duas categorias, covid e normal.

## Bibliotecas Utilizadas
 
- 📁 [os](https://docs.python.org/pt-br/3/library/os.html)
  - Biblioteca utilizada para manipulação de arquivos e diretórios.

- 📷 [cv2](https://pypi.org/project/opencv-python/)
  - Biblioteca utilizada para manipulação de imagens.

- 🧮 [numpy](https://pypi.org/project/numpy/)
  - Biblioteca utilizada para manipulação de matrizes.

- 🤖 [sklearn](https://pypi.org/project/scikit-learn/)
  - Biblioteca utilizada para implementação dos classificadores.

- 🔄 [progressbar](https://pypi.org/project/progress/)
  - Biblioteca utilizada para implementação de barra de progresso.

- ⏰ [time](https://docs.python.org/3/library/time.html)
  - Biblioteca utilizada para implementação de contagem de tempo.

- 📸 [skimage](https://pypi.org/project/scikit-image/)
  - Biblioteca utilizada para implementação do descritor LBP.

- 📂 [splitfolders](https://pypi.org/project/split-folders/)
  - Biblioteca utilizada para separação das imagens em pastas de treino e teste.

- 📊 [matplotlib](https://pypi.org/project/matplotlib/)
  - Biblioteca utilizada para implementação de gráficos.

- 🐼 [pandas](https://pypi.org/project/pandas/)
  - Biblioteca utilizada para manipulação de dados.

- 🗓️ [datetime](https://docs.python.org/3/library/datetime.html)
  - Biblioteca utilizada para manipulação de datas e horas.


## Classificadores e Acurácias

Para avaliar a eficácia do descritor implementado, foram utilizados os seguintes classificadores:

O primeiro classificador utilizado foi o Multilayer Perceptron (MLP), o mesmo é uma rede neural artificial semelhante à perceptron, mas com múltiplas camadas ocultas.

O segundo classificador utilizado foi o Support Vector Machine (SVM), o mesmo é um modelo de aprendizado supervisionado que analisa os dados e reconhece padrões.

Por fim, o terceiro classificador utilizado foi o Random Forest, o mesmo é um algoritmo de aprendizado supervisionado que cria de forma aleatória várias árvores de decisão e combina os resultados de todas elas para obter o resultado final.

Os resultados obtidos foram:
1. **Multilayer Perceptron (MLP)**
   - Acurácia: 94.64%

2. **Support Vector Machine (SVM)**
   - Acurácia: 80.36%

2. **Random Forest**
   - Acurácia: 96.43%

Os resultados obtidos foram muito bons, mas o classificador que apresentou o melhor resultado foi o Random Forest, com uma acurácia de 96.43%.

## Instruções de Uso
Para a executação do projeto, é necessário seguir as seguintes etapas:
1. Ter o Python 3 instalado.
2. Ter o ambiente de desenvolvimento configurado.
3. Instalar as bibliotecas necessárias.
4. Clonar o repositório do projeto.
5. Baixar o dataset e descompactar o mesmo na pasta images_full.
6. Renomear as imagens e separar as mesmas em pastas de treino e teste:
   - Executar o arquivo *data_spliting.py*.
   - Para executar o algoritmo, é necessário abrir o arquivo e pressionar as teclas Ctrl + F5.
   - Aguarde a finalização para prosseguir.
7. Extrair características das imagens utilizando o descritor LBP:
   - Para executar o arquivo *localBinaryPatterns_FeatureExtraction*.
   - Para executar o algoritmo, é necessário abrir o arquivo e pressionar as teclas Ctrl + F5.
   - Aguarde a finalização para prosseguir.
8. Classificação das imagens utilizando os classificadores:
   - Existem 3 classificadores implementados, os mesmo podem ser executador de forma individual ou todos de uma vez por meio do arquivo *run_all_classifiers.py*.
   - Para executar o algoritmo, é necessário abrir o arquivo e pressionar as teclas Ctrl + F5.
   - Por fim, ao final da classificação será gerado uma imagem contendo a matriz de confusão para os classificadores escolhidos e suas respectivas acurácias.
