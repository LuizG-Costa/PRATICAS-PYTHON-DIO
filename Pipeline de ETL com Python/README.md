# 📊 Análise de Movimentações de Funcionários com Pandas

Projeto de treino para manipulação e análise de dados com a biblioteca **Pandas** em Python.

---

## 📋 Descrição

Este projeto realiza a leitura, transformação e filtragem de uma planilha de movimentações de funcionários, exportando o resultado final em um novo arquivo CSV.

---

## 🗂️ Estrutura do Projeto

```
📁 projeto/
├── main.ipynb                              # Notebook principal com toda a análise
├── Movimentacoes_Consolidado_Finalizado.csv   # Planilha de entrada
├── Movimentacoes_Consolidadas_Filtradas.csv   # Planilha de saída (resultado)
└── README.md
```

---

## 🔄 Fluxo da Análise

1. **Importação da biblioteca** — carregamento do Pandas
2. **Leitura da planilha** — leitura do CSV com encoding UTF-8 e separador `;`
3. **Inspeção dos dados** — uso de `.info()` e `.head()` para entender a estrutura
4. **Transformação de tipos** — conversão da coluna `data` de `string` para `datetime`
5. **Filtros** — filtragem por cargo (sindicato) e escala de trabalho
6. **Exportação** — salvamento do DataFrame filtrado em novo arquivo CSV

---

## 🧪 Principais Técnicas Utilizadas

| Técnica | Método |
|---|---|
| Leitura de CSV | `pd.read_csv()` |
| Inspeção de dados | `df.info()`, `df.head()` |
| Conversão de tipo de data | `pd.to_datetime()` |
| Filtro simples | `df[df["coluna"] == "valor"]` |
| Filtro com múltiplas condições | `df[(condição1) & (condição2)]` |
| Filtro com lista de valores | `df["coluna"].isin([...])` |
| Exportação de CSV | `df.to_csv()` |

---

## 📦 Colunas do Dataset

| Coluna | Descrição |
|---|---|
| `data` | Data da movimentação |
| `matricula` | Matrícula do funcionário |
| `descricaoFuncionarioCargo` | Cargo do funcionário |
| `descricaoFuncionarioEscalaTrabalho` | Escala de trabalho |
| `descricaoFuncionarioSindicato` | Sindicato vinculado |
| `descricaoPostoTrabalho` | Posto de trabalho |

---

## ▶️ Como Executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
   ```

2. Instale as dependências:
   ```bash
   pip install pandas
   ```

3. Abra o notebook:
   ```bash
   jupyter notebook main.ipynb
   ```

---

## 🛠️ Tecnologias

- Python 3.x
- [Pandas](https://pandas.pydata.org/)
- Jupyter Notebook
