# 📚 Importação de Módulos e Bibliotecas em Python

Abaixo estão alguns módulos e bibliotecas úteis em Python, organizados com ícones para facilitar a identificação.

A biblioteca padrão do Python
A Biblioteca Padrão do Python é uma extensa coleção de códigos Python que geralmente vem junto com o Python. Ela inclui uma variedade de módulos, cada um com programação pré-construída centrada em um tipo específico de tarefa.

Por exemplo, você foi apresentado anteriormente aos seguintes módulos da Biblioteca Padrão do Python:

- O módulo re, que fornece funções usadas para pesquisar padrões em arquivos de log
- O módulo csv, que fornece funções usadas ao trabalhar com arquivos .csv
- Os módulos glob e os, que fornecem funções usadas na interação com a linha de comando
- Os módulos time e datetime, que fornecem funções usadas ao trabalhar com registros de data e hora

Outro módulo da Biblioteca Padrão Python é o statistics. O módulo statistics inclui funções usadas no cálculo de estatísticas relacionadas a dados numéricos. Por exemplo, mean() é uma função no módulo statistics que recebe dados numéricos como entrada e calcula sua média (ou average). Além disso, median() é uma função no módulo statistics que recebe dados numéricos como entrada e calcula sua mediana (ou valor médio).

## 📌 Como importar módulos da biblioteca padrão do Python
Para acessar os módulos da biblioteca padrão do Python, é necessário importá-los. Você pode optar por importar um módulo completo ou importar apenas funções específicas de um módulo.

### 🔹 Importando um Módulo inteiro
Para importar um módulo inteiro da Biblioteca Padrão Python, use a palavra-chave `import`. A palavra-chave `import` procura um Módulo ou uma biblioteca em um sistema e o adiciona ao ambiente Python local. Após `import`, especifique o nome do Módulo a ser importado. Por exemplo, você pode especificar `import statistics` para importar o módulo statistics. Isso importará todas as funções dentro do módulo statistics para uso posterior em seu código.

Por exemplo, talvez você queira usar a função `mean()` do módulo statistics para calcular o número médio de tentativas de login com falha por mês para um determinado usuário. No bloco de código a seguir, o número total de tentativas de login com falha para cada um dos doze meses é armazenado em uma lista chamada `monthly_failed_attempts`. Execute esse código e analise como `mean()` pode ser usado para calcular a média desses totais mensais de login com falha e armazená-la em `mean_failed_attempts`:

```python
import statistics
monthly_failed_attempts = [20, 17, 178, 33, 15, 21, 19, 29, 32, 15, 25, 19]
mean_failed_attempts = statistics.mean(monthly_failed_attempts)
print("mean:", mean_failed_attempts)
```

A saída retorna uma média de `35.25`. Você pode notar o valor discrepante de `178` e deseja encontrar o valor médio também. Para fazer isso por meio da função `median()`, você pode usar o código a seguir:

```python
import statistics
monthly_failed_attempts = [20, 17, 178, 33, 15, 21, 19, 29, 32, 15, 25, 19]
median_failed_attempts = statistics.median(monthly_failed_attempts)
print("median:", median_failed_attempts)
```

Isso lhe dá o valor de `20.5`, que também pode ser útil para analisar as estatísticas de tentativas de login fracassadas do usuário.

> **Observação:** ao importar um módulo inteiro da Python Standard Library, você precisa identificar o nome do módulo com a função ao chamá-la. Você pode fazer isso colocando o nome do Módulo seguido de um ponto (.) antes do nome da função. Por exemplo, os blocos de código anteriores usam `statistics.mean()` e `statistics.median()` para chamar essas funções.

### 🔹 Importação de funções específicas de um Módulo
Para importar uma função específica da biblioteca padrão Python, você pode usar a palavra-chave `from`. Por exemplo, se quiser importar apenas a função `median()` do módulo statistics, você pode escrever:

```python
from statistics import median
```

Para importar várias funções de um Módulo, você pode separar as funções que deseja importar com uma vírgula. Por exemplo:

```python
from statistics import mean, median
```

Isso importa as funções `mean()` e `median()` do módulo statistics.

Um detalhe importante a ser observado é que, se você importar funções específicas de um módulo, não precisará mais especificar o nome do módulo antes dessas funções. Você pode examinar isso no código a seguir, que importa especificamente apenas as funções `median()` e `mean()` do módulo statistics e executa os mesmos cálculos que os exemplos anteriores:

```python
from statistics import mean, median
monthly_failed_attempts = [20, 17, 178, 33, 15, 21, 19, 29, 32, 15, 25, 19]
mean_failed_attempts = mean(monthly_failed_attempts)
print("mean:", mean_failed_attempts)
median_failed_attempts = median(monthly_failed_attempts)
print("median:", median_failed_attempts)
```

Agora, não é mais necessário especificar `statistics.mean()` ou `statistics.median()`, podendo usar apenas `mean()` e `median()`.

## 📦 Bibliotecas Externas
Além da biblioteca padrão do Python, também é possível fazer download de bibliotecas externas e incorporá-las ao seu código Python. Por exemplo, anteriormente você foi apresentado à **Beautiful Soup (bs4)** para analisar arquivos HTML e à **NumPy (numpy)** para matrizes unidimensionais e cálculos matemáticos. Antes de usá-las em um Notebook Jupyter ou em um ambiente do Google Colab, é necessário instalá-las primeiro.

Para instalar uma biblioteca, como a `numpy`, em qualquer ambiente, você pode executar a seguinte linha antes de importar a biblioteca:

```sh
pip install numpy
```

Isso instala as bibliotecas para que você possa usá-las em seu código Python.

Depois que uma biblioteca for instalada, você poderá importá-la diretamente para o Python usando a palavra-chave `import` de forma semelhante à usada para importar módulos da Biblioteca Padrão do Python. Por exemplo, após a instalação do `numpy`, você pode usá-lo assim:

```python
import numpy as np
```

## 🔥 Principais Conclusões
- A **Python Standard Library** contém muitos módulos que você pode importar, incluindo `re`, `csv`, `os`, `glob`, `time`, `datetime` e `statistics`.
- Para importar esses módulos, use a palavra-chave `import`.
- A sintaxe varia se você quiser importar o módulo inteiro ou apenas funções específicas dele.
- **Bibliotecas externas** também podem ser importadas para o Python, mas elas precisam ser instaladas primeiro usando `pip install <nome_da_biblioteca>`.

🚀 **Agora você está pronto para explorar mais módulos e bibliotecas no Python!**
