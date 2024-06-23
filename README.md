# Título e descrição do Projeto:

    Projeto prático Processamento de Imagens

    O sistema utiliza principalmente a técnica de Padrões Binários Locais (LBP) para extrair características significativas das imagens. Essa técnica é fundamental para capturar informações detalhadas e distintivas que são essenciais para o processo de classificação das imagens. Essas características são essenciais para capturar informações únicas e relevantes de cada imagem. Além disso, os rótulos associados às imagens são convertidos para valores numéricos, o que facilita o treinamento dos modelos de aprendizado de máquina.

    Após o pré-processamento, o sistema procede com o treinamento de diferentes modelos de classificação, incluindo MLP (Perceptron Multicamadas), Random Forest e SVM (Máquina de Vetores de Suporte). Esses modelos utilizam as características extraídas das imagens e os rótulos numéricos correspondentes para aprender a distinguir entre diferentes classes de imagens.

    Para avaliar a eficácia dos modelos treinados, são utilizadas imagens separadas exclusivamente para testes. As previsões geradas pelos modelos são então comparadas com os rótulos reais das imagens de teste, utilizando uma matriz de confusão. Essa matriz fornece uma medida precisa da precisão de cada modelo na tarefa de classificação das imagens.

## Equipe

- Jacó Cabral De Jesus
- João Henrique Rossato Filho


## Descrição do(s) descritor(es) implementado
Nesse projeto foi utilizado o Local binary patterns (LBP) Padrões Binários Locais em português.

O método de Padrões Binários Locais (LBP) é uma técnica de processamento de imagem que detecta características distintas da textura de uma imagem. Ele compara cada pixel da imagem com seus vizinhos, gerando um histograma que mostra como esses padrões binários estão distribuídos na imagem. Isso ajuda a identificar áreas onde a textura é uniforme ou variada, sendo útil para reconhecer padrões repetitivos ou texturas complexas em imagens. Essa capacidade é fundamental para classificar e reconhecer objetos com precisão.

Repositório do projeto:
   AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA

## Classificador e acurácia:    

### Local Binary Pattern:

- Multilayer Perceptron: 89.28%
- Random Forest: 96.42%
- Support Vector Machine: 87.5%


 
##  Instruções de uso:
- Passo 1

    Antes de extrair as features é necessário conferir se as pastas features_labels/test e features_labels/train estão vazias.

- Passo 2

    É preciso alimentar os sistema adicionando as imagens na pasta: ./images_full

- Passo 3

    É preciso instalar as seguintes dependencias:
    
    pip install scikit-image 

    pip install progress

    pip install opencv-python

    pip install scikit-learn 

    pip install matplotlib   

    pip install split-folders

- Passo 4 
    
    É preciso executar o arquivo data_splitting.py para separar as imagens nos diretorios corretos para o pleno funcionamento do sistema

- Passo 5

    Executar o arquivo grayHistogram_FeatureExtraction.py para gerar as features que serão armazenadas nas pastas features_labels/test e features_labels/train (por isso devem estar vazias)

- Passo 6 

    Executar o arquivo run_all_classifiers.py para realizar as previsões e obeter as matrizes e as acuracias.