# Análise de Dados para Pequenos Negócios: Um Guia Prático e Replicável

Este projeto tem como objetivo fornecer um guia prático para análise de dados de vendas, utilizando uma planilha do Excel como base. Você pode substituir os dados da planilha pelos seus próprios dados de vendas, desde que sigam a mesma estrutura.

---

## Estrutura do Exemplo

A planilha de exemplo que vamos usar contém dados de **shoppings e produtos**. Ela está organizada da seguinte maneira:

| Data       | Loja               | Produto        | Quantidade | Valor Unitário | Valor Final |
|------------|--------------------|----------------|------------|----------------|-------------|
| 12/1/2019  | Iguatemi Campinas  | Bermuda Estampa| 1          | R$ 169,00      | R$ 169,00   |
| 12/1/2019  | Iguatemi Esplanada | Bermuda Xadrez | 1          | R$ 155,00      | R$ 155,00   |
| 12/1/2019  | Norte Shopping     | Bermuda        | 2          | R$ 150,00      | R$ 300,00   |

### Estrutura das Colunas:
- **Data**: A data da venda.
- **Loja**: Nome da loja onde o produto foi vendido.
- **Produto**: Nome do produto.
- **Quantidade**: Quantidade do produto vendido.
- **Valor Unitário**: Valor do produto por unidade.
- **Valor Final**: Total da venda (Quantidade x Valor Unitário).

---

## Requisitos

Vamos utilizar Python 3 para a análise de dados, com o ambiente de desenvolvimento configurado com **venv** e ferramentas como **Jupyter Notebook** e **JupyterLab**.

### Pré-requisitos

Certifique-se de ter os seguintes pré-requisitos instalados no seu sistema:
- **Python 3** (Versão 3.7 ou superior).
- **pip** (gerenciador de pacotes do Python).

### 1. Instalar Python 3

Se você ainda não tem o Python 3 instalado, baixe e instale a versão mais recente do [site oficial do Python](https://www.python.org/downloads/).

### 2. Clonar o Repositório

Para começar, clone o repositório para o seu computador. Abra o terminal e execute o seguinte comando:

```bash
git clone https://github.com/BrunoHoinacki/Analise-de-dados-pequenas-empresas.git
```

Após o clone, entre no diretório do projeto:

```bash
cd Analise-de-dados-pequenas-empresas
```

---

### 3. Criar o Ambiente Virtual

1. No diretório do projeto, crie um ambiente virtual com o comando:

   ```bash
   python -m venv .venv
   ```

2. Ative o ambiente virtual:

   - **Windows**:
     ```bash
     .\.venv\Scripts\activate
     ```

   - **macOS/Linux**:
     ```bash
     source .venv/bin/activate
     ```

   Você verá o nome do ambiente `(venv)` no prompt de comando, indicando que o ambiente virtual está ativo.

### 4. Instalar as Dependências

1. Dentro do ambiente virtual, instale as dependências necessárias com o comando:

   ```bash
   pip install -r requirements.txt
   ```

   Se você não tiver um arquivo `requirements.txt` ainda, crie um com os seguintes pacotes:

   ```txt
   pandas
   numpy
   matplotlib
   seaborn
   jupyterlab
   notebook
   openpyxl
   ```

2. Após rodar o comando acima, todos os pacotes necessários para o projeto serão instalados.

### 5. Rodar o Jupyter Notebook ou JupyterLab

Com o ambiente virtual ativado e as dependências instaladas, você pode rodar o **Jupyter Notebook** ou **JupyterLab**.

- Para iniciar o **Jupyter Notebook**, use o seguinte comando:

  ```bash
  jupyter notebook
  ```

  Isso abrirá o Jupyter em seu navegador padrão, onde você poderá criar e editar notebooks.

- Para iniciar o **JupyterLab**, use o comando:

  ```bash
  jupyter lab
  ```

  JupyterLab oferece uma interface mais robusta para trabalhar com notebooks e outros arquivos.

---

## Estrutura do Projeto

- **README.md**: Este arquivo, contendo instruções e informações sobre o projeto.
- **Vendas.xlsx**: A planilha de exemplo com os dados de vendas.
- **Análise-de-dados-pequenas-empresas.ipynb**: O Jupyter Notebook onde a análise será realizada.

---

## Como Utilizar

1. **Substituir os dados de exemplo**: Para realizar a análise com seus próprios dados, basta substituir os dados na planilha **Vendas.xlsx** pela sua base de dados.
2. **Carregar a planilha no Notebook**: No Jupyter Notebook ou JupyterLab, importe os dados utilizando o pandas:

   ```python
   import pandas as pd

   # Carregar a planilha de dados
   dados = pd.read_excel('Vendas.xlsx')
   dados.head()
   ```

3. **Análise dos dados**: Após carregar os dados, você pode começar a analisar as vendas, calcular totais, médias e até criar gráficos.

---

## Conclusão

Este projeto é uma maneira prática e simples de aplicar análise de dados em dados reais de pequenas empresas. Com as ferramentas adequadas e a organização correta dos dados, é possível obter insights valiosos que podem ajudar na tomada de decisões.

Se você tiver dúvidas ou sugestões, sinta-se à vontade para abrir uma **issue** no repositório!
