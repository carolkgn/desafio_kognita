## Desafio Kognita
**********


![Imagem](./img.png)
************
### Árvore de diretórios

```markdown
├── _data
│   └── dataset_2021-5-26-10-14.csv
├── docs
│   ├── 2089-6809-1-PB.pdf
│   └── README.md
├── environment.yml
├── Notebooks
│   ├── Análise Exploratória.ipynb
│   ├── modelo_credit_score
│   ├── Simulador de crédito.ipynb
│   └── X-Health - Pipeline de modelagem.ipynb
├── README.md
└── requirements.txt
```
***********
### Descrição do exercício

- **Contexto geral** - A empresa X-Health atua no comércio B2B vendendo dispositivos eletrônicos voltados para saúde com amplo espectro de preços, e de variada sofisticação/complexidade. 
  
- **Sobre as vendas** - As vendas são feitas à crédito: o cliente B2B faz seu pedido e paga (à vista ou em várias parcelas, conforme o combinado pelo time de vendas) num tempo futuro pré-determinado.
  
- **O problema** - O time financeiro da X-Health tem observado um número indesejável de não-pagamentos ("default" ou calote, em bom português).

- **O objetivo** - Querem de alguma forma minimizar esse fenômeno. Desejam um algoritmo que seja capaz de inferir a probabilidade de default para um dado pedido.
*********
### Textos consultados para resolução do exercício

- COELHO, Felipe Fernandes; DE LIMA AMORIM, Daniel Penido; DE CAMARGOS, Marcos Antônio. Analisando métodos de machine learning e avaliação do risco de crédito. **Revista Gestão & Tecnologia**, v. 21, n. 1, p. 89-116, 2021.
- KOEHRSEN, Will. An Implementation and Explanation of the Random Forest in Python: a guide for using and understanding the random forest by building up from a single decision tree.. A guide for using and understanding the random forest by building up from a single decision tree. 2018. **Towards Data Science**. Disponível em: https://towardsdatascience.com/an-implementation-and-explanation-of-the-random-forest-in-python-77bf308a9b76. Acesso em: 10 set. 2021

*************
### Descrição das pastas do repositório
**************

**Pasta**| **Descrição**|
---------|--------------|
_data| Pasta contendo a base de dados utilizada no exercício|
docs| Pasta contendo o arquivo original de descrição do exercício e o pdf de um dos textos consultados|
Notebooks| Pasta contendo os notebooks de análise, pipeline do modelo e simulação|

******

### Descrição dos arquivos do repositório
****
**Arquivo**| **Descrição**|
------------|--------------|
requirements.txt| Arquivo contendo as dependências utilizadas no projeto|
environment.yml| Arquivo contendo configurações e depemdências necessárias para recriação do ambiente|
*Notebooks*/X-Health - Pipeline de modelagem.ipynb| Notebook contendo o pipeline de limpeza, preparação, modelagem e exportação de modelo|
*Notebooks*/Simulador de crédito.ipynb| Notebook contendo importação, carregamento e testagem simulada do modelo|
*Notebooks*/Análise Exploratória.ipynb| Notebook contendo a análise exploratória da base|
*docs*/README.md| Documento contendo o enunciado original do projeto|
*docs*/2089-6809-1-PB.pdf| PDF do artigo de Coelho et. al (2021).
*_data*/dataset_2021-5-26-10-14.csv| Arquivo CSV com a base de dados utilizada no projeto|
**********

### Como preparar o ambiente para executar o projeto
********

Clone este repositório no local desejado com o comando:

```bash
git clone https://github.com/carolkgn/desafio_kognita.git
```

Em seguida, em uma terminal navegue até o diretório onde o repositório foi clonado e, dentro da pasta principal **desafio_kognita**, digite:

```bash
conda env create -f environment.yml
```
Aguarde até que o Anaconda crie o ambiente e instale todas as dependências do arquivo requirements.txt.

Se necessário, é possível instalar as dependências manualmente com o comando:

```bash
pip install -r requirements.txt
```
Após a realização dos passos anteriores digite:

```bash
conda activate credto
```
Isso ativará o ambiente do projeto. Em seguida, digite:

```bash
jupyter-lab
```

ou

```bash
jupyter-notebook
```
para abrir e rodar os notebooks localamente.

**Observação**:
Antes de fazer a instalação do ambiente e das dependências do projeto, certifique-se de possuir uma versão no Anaconda previamente instalada em sua máquina.

É possível encontrar mais informações sobre o Anaconda aqui: https://www.anaconda.com/products/individual-d

*************

[![Made withJupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)](https://jupyter.org/try)