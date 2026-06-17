# ClearBank - Análise Financeira com Python

## Descrição

Este projeto foi desenvolvido como desafio final do módulo de Análise de Dados com Python. O objetivo é realizar a leitura, validação e análise de transações financeiras armazenadas em um arquivo CSV, gerando relatórios mensais, identificando transações suspeitas e exportando os resultados em formato JSON.

Além da implementação utilizando apenas bibliotecas nativas do Python, o projeto também apresenta uma versão alternativa utilizando a biblioteca Pandas para comparação dos resultados.

---

## Estrutura do Projeto

```
clearbank-analise/
│
├── desafio-final.ipynb      # Notebook principal
├── transacoes.csv           # Arquivo de entrada
├── relatorio.json           # Relatório gerado automaticamente
├── grafico.png              # Gráfico do saldo mensal
├── analise_pandas.py        # Implementação utilizando Pandas
└── README.md                # Documentação do projeto
```

---

## Tecnologias Utilizadas

- Python 3.10+
- csv
- json
- datetime
- pandas (opcional)
- matplotlib (opcional)

---

## Funcionalidades

- Leitura do arquivo CSV utilizando `csv.DictReader`.
- Validação e limpeza dos dados.
- Tratamento de exceções utilizando `try/except`.
- Conversão de datas com `datetime`.
- Agrupamento das transações por mês.
- Cálculo de métricas financeiras mensais:
  - Quantidade de transações;
  - Total de créditos;
  - Total de débitos;
  - Saldo mensal;
  - Média por transação;
  - Maior valor;
  - Menor valor.
- Identificação de transações suspeitas (acima de R$ 10.000,00).
- Geração do arquivo `relatorio.json`.
- Exibição de relatório formatado no terminal.
- Implementação alternativa utilizando Pandas.
- Geração de gráfico com Matplotlib.

---

## Como Executar

1. Clone o repositório:

```bash
git clone https://github.com/SEU-USUARIO/clearbank-analise.git
```

2. Acesse a pasta do projeto:

```bash
cd clearbank-analise
```

3. Instale as bibliotecas opcionais (caso ainda não possua):

```bash
pip install pandas matplotlib
```

4. Execute o notebook `desafio-final.ipynb` ou abra-o no Google Colab.

5. Execute todas as células em sequência.

---

## Arquivos Gerados

Após a execução serão gerados automaticamente:

- `relatorio.json`
- `grafico.png`

Caso execute o arquivo `analise_pandas.py`, será exibido no terminal um relatório equivalente utilizando a biblioteca Pandas.

---

## Estrutura do Arquivo CSV

O arquivo `transacoes.csv` possui as seguintes colunas:

| Coluna | Descrição |
|---------|-----------|
| id | Identificador da transação |
| data | Data da transação |
| cliente_id | Código do cliente |
| tipo | Crédito ou Débito |
| valor | Valor da transação |
| descricao | Descrição da operação |
| categoria | Categoria da transação |

---

## Requisitos Atendidos

- Leitura utilizando módulo nativo `csv`.
- Validação dos registros.
- Organização em funções.
- Tratamento de exceções.
- Manipulação de datas.
- Agrupamento por mês.
- Relatório financeiro.
- Identificação de transações suspeitas.
- Exportação para JSON.
- Implementação alternativa com Pandas.
- Gráfico utilizando Matplotlib.

---

## Autor

Rodrigo Garcia Abegão

Projeto desenvolvido para fins acadêmicos como desafio final da disciplina de Análise de Dados com Python.
