# Análise dos Preços da Gasolina em Minas Gerais Durante a Pandemia de COVID-19

Este projeto tem como objetivo analisar a variação do preço da gasolina no estado de Minas Gerais (MG) durante a pandemia de COVID-19, com foco em três momentos distintos:

- Antes do lockdown (até 15 de março de 2020)  
- Durante o lockdown e o período de baixa atividade econômica (ao longo de 2020)  
- Pós-vacinação, entre março e julho de 2021

O estudo foi motivado pelo caso de **José**, empresário dono de uma frota de táxis em Belo Horizonte, preocupado com os impactos dos preços dos combustíveis em seu negócio durante a pandemia.

## 🗂 Dados Utilizados

Os dados foram obtidos no site da **Agência Nacional do Petróleo, Gás Natural e Biocombustíveis (ANP)** e referem-se aos preços praticados por diversos revendedores em todo o Brasil.

Foram utilizados os seguintes arquivos:

- `ca-2020-01.csv` (1º semestre de 2020)  
- `ca-2020-02.csv` (2º semestre de 2020)  
- `ca-2021-01.csv` (1º semestre de 2021)

Apenas os registros do produto "GASOLINA" no estado de Minas Gerais (MG) foram considerados.

📥 Link para download dos dados:  
[Série histórica de preços de combustíveis – ANP](https://www.gov.br/anp/pt-br/centrais-de-conteudo/dados-abertos/serie-historica-de-precos-de-combustiveis)

## 🛠 Tecnologias e Bibliotecas

- Python 3  
- Pandas  
- Seaborn  
- Matplotlib  
- Google Colab

## 🔍 Metodologia

1. **Importação e união dos dados:** os arquivos CSV foram carregados e combinados em um único DataFrame.  
2. **Limpeza dos dados:** conversão de datas, tratamento de separadores decimais e remoção ou substituição de valores ausentes.  
3. **Filtragem:** seleção apenas de registros com gasolina no estado de MG.  
4. **Análise estatística:** cálculo das médias de preços, valor mínimo e valor máximo registrados.  
5. **Visualização:** geração de um gráfico de linha representando a evolução dos preços ao longo do período.

## 📈 Resultados

- 📌 Média antes do lockdown (até 15/03/2020): **R$ 4,84**  
- 📌 Média entre março e julho de 2021: **R$ 5,85**  
- 📉 Menor valor registrado: **R$ 3,56**  
- 📈 Maior valor registrado: **R$ 7,00**

*Esses valores podem variar conforme a base de dados atualizada utilizada na execução.*

## ▶️ Como Executar

1. **Baixe os arquivos de dados:**
   - Acesse: [Série histórica de preços de combustíveis – ANP](https://www.gov.br/anp/pt-br/centrais-de-conteudo/dados-abertos/serie-historica-de-precos-de-combustiveis)
   - Baixe os seguintes arquivos:
     - `ca-2020-01.csv`
     - `ca-2020-02.csv`
     - `ca-2021-01.csv`

<img width="964" height="454" alt="ANP-Download" src="https://github.com/user-attachments/assets/b4b85f2e-9955-45e2-afd8-233d5b4dbc82" />

3. **Abra o Google Colab:**
   - Link: [https://colab.research.google.com](https://colab.research.google.com)

4. **Crie um novo notebook:**
   - Clique em **Arquivo > Novo notebook**

5. **Cole o código de análise no notebook**  
   * O código está no arquivo `analise_preco_gasolina.ipynb`

6. **Execute o notebook:**
   - Clique em **Executar**
   - Quando solicitado, selecione os três arquivos `.csv` de uma só vez

7. **Veja os resultados:**
   - As médias e valores serão exibidos no console
   - Um gráfico mostrará a evolução dos preços da gasolina ao longo do tempo
