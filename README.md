# Análise Estatística e Testes de Hipóteses

Este repositório contém uma análise de dados focada em testes de hipóteses, utilizando datasets para responder a questões de negócio relacionadas com testes A/B e estatísticas de pacientes de um hospital. O projeto demonstra a aplicação de vários métodos estatísticos para extrair conclusões significativas a partir dos dados.

## Contexto do Projeto

### A análise está dividida em duas partes principais:
1.	Teste A/B: Análise da base de dados `experimento_teste_ab.csv` para determinar qual de duas versões (A ou B) tem a maior taxa de conversão e para calcular o tamanho de amostra necessário para futuros testes.

2.	Análise de Pacientes: Utilização da base de dados `pacientes.csv` para aplicar testes de hipóteses (Teste t, ANOVA, Qui-quadrado, etc.) e responder a questões sobre a relação entre variáveis como pressão arterial, idade, gênero e etnia.

#### Questões Investigadas:
Este projeto responde às seguintes perguntas com base nos dados fornecidos:

•	Qual cenário (A ou B) possui a maior taxa de conversão?

•	Qual é a diferença na pressão arterial média entre fumantes e não fumantes?

•	Existe uma diferença significativa na pressão arterial entre diferentes grupos étnicos?

•	Há uma relação entre o género dos pacientes e a presença de condições de saúde adicionais?

•	A distribuição da pressão arterial na população segue uma distribuição normal? (Entre outras questões detalhadas no notebook e no relatório.)

### Estrutura do Repositório:

#### O projeto está organizado da seguinte forma:

•	/data: Contém os datasets originais (experimento_teste_ab.csv e pacientes.csv).

•	/notebook: Inclui o Jupyter Notebook Testes_de_Hipoteses.ipynb com todo o código para a limpeza de dados, análise exploratória e aplicação dos testes estatísticos.

•	/relatorio: Contém o relatório final Estatística - Teste de Hipóteses.pdf que resume as questões e conclusões do estudo.

•	/modelo: Armazena um ficheiro analise_estatistica.pkl simbólico, indicando que este projeto não envolve modelagem preditiva.

•	requirements.txt: Lista de todas as bibliotecas Python necessárias para reproduzir o ambiente e executar a análise.

•	README.md: Este guia, com a documentação completa do projeto.

### Como Instalar e Executar o Projeto:

Siga os passos abaixo para configurar o ambiente e executar a análise no seu computador.

#### Pré-requisitos

•	Python 3.8 ou superior

•	pip (gestor de pacotes do Python)

*1. Clonar o Repositório*

Clone este repositório para a sua máquina local usando o seguinte comando no seu terminal:

    git clone <URL-DO-SEU-REPOSITÓRIO-AQUI>
    cd <NOME-DA-PASTA-DO-REPOSITÓRIO>

*2. Criar um Ambiente Virtual (Recomendado)*

Para isolar as dependências do projeto, crie e ative um ambiente virtual:

##### Para Windows
    python -m venv venv
    venv\Scripts\activate

##### Para macOS/Linux
    python3 -m venv venv
    source venv/bin/activate

*3. Instalar as Dependências*

Com o ambiente virtual ativado, instale todas as bibliotecas necessárias:

    pip install -r requirements.txt

*4. Executar a Análise*

Para visualizar e reexecutar a análise, inicie o Jupyter Notebook:

    jupyter notebook notebook/Testes_de_Hipoteses.ipynb

#### Ferramentas Utilizadas

•	Linguagem: Python 3

•	Bibliotecas Principais:

- Pandas & Numpy: para manipulação e análise de dados.

- Matplotlib & Seaborn: para visualização de dados.

- Scipy.stats: para a aplicação dos testes estatísticos.

- Jupyter Notebook: como ambiente de desenvolvimento interativo.
