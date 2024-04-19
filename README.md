# An-lise-de-dados-com-Python-e-Pandas

A biblioteca **Pandas** é realmente uma ferramenta poderosa para análise de dados em Python. Com ela, podemos realizar diversas operações como:

- **Carregar dados** de diferentes fontes como CSV, Excel, SQL, entre outros.
- **Manipular e limpar** os dados para prepará-los para análise.
- **Combinar** dados de múltiplas fontes.
- Realizar **cálculos estatísticos** e **agregações**.
- **Visualizar** os dados com a ajuda de outras bibliotecas como Matplotlib ou Seaborn.

Aqui está um exemplo simples de como podemos carregar um arquivo CSV e visualizar as primeiras linhas de dados usando Pandas:

```python
import pandas as pd

# Carregar os dados do arquivo CSV
df = pd.read_csv('caminho_para_seu_arquivo.csv')

# Visualizar as primeiras 5 linhas do DataFrame
print(df.head())
```

Como filtrar dados com a biblioteca Pandas é uma tarefa comum e útil. Aqui está um exemplo de como podemos filtrar linhas de um `DataFrame` com base em condições específicas:

```python
import pandas as pd

# Supondo que você já tenha um DataFrame chamado 'df'

# Filtrar linhas onde a coluna 'idade' é maior que 30
df_filtrado = df[df['idade'] > 30]

# Filtrar linhas onde a coluna 'cidade' é igual a 'São Paulo'
df_filtrado_sp = df[df['cidade'] == 'São Paulo']

# Também podemos combinar múltiplas condições
df_filtrado_complexo = df[(df['idade'] > 30) & (df['cidade'] == 'São Paulo')]

# Visualizar o DataFrame filtrado
print(df_filtrado_complexo.head())
```

Neste exemplo, `df['idade'] > 30` é a condição para filtrar as linhas onde a idade é maior que 30. O operador `&` é usado para combinar condições, e os parênteses são necessários para garantir que as operações sejam realizadas na ordem correta.

http://colab.research.google.com/notebooks/intro.ipynb
