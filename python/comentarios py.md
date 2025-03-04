# Garantir a Sintaxe e a Legibilidade Adequadas em Python

## 📂 Introdução
Anteriormente, você foi apresentado ao guia de estilo **PEP 8** e suas diretrizes para programadores que trabalham em Python. Também aprendeu sobre a importância da **indentacão correta** e do uso de **comentários** para tornar o código mais legível.

Esta leitura explora essas ideias e também foca em aspectos comuns da **sintaxe** do Python para garantir que seu código seja executado corretamente.

---
## 💡 Comentários
Os comentários são notas que programadores deixam no código para explicar sua intenção. Eles tornam o código mais fácil de ler e entender.

### 📃 Comentários de Linha Única
Os comentários de linha única são precedidos pelo símbolo **#**. O PEP 8 recomenda manter cada linha com **menos de 79 caracteres**.

Exemplo:
```python
# Exibe os elementos da lista 'computer_assets'
computer_assets = ["laptop1", "desktop20", "smartphone03"]
for asset in computer_assets:
    print(asset)
```

### 📄 Comentários de Múltiplas Linhas
Para comentários mais longos, use várias linhas com **#** ou **docstrings** com aspas triplas.

Exemplo com **#**:
```python
# A função remaining_login_attempts() recebe dois parâmetros inteiros,
# o número máximo de tentativas de login e o total de tentativas feitas.
# Retorna um inteiro representando as tentativas restantes.
def remaining_login_attempts(maximum_attempts, total_attempts):
    return maximum_attempts - total_attempts
```

Exemplo com **docstrings**:
```python
def remaining_login_attempts(maximum_attempts, total_attempts):
    """
    Calcula o número de tentativas de login restantes.
    Parâmetros:
    - maximum_attempts (int): Tentativas máximas permitidas.
    - total_attempts (int): Tentativas já realizadas.
    Retorna:
    - (int) Tentativas restantes.
    """
    return maximum_attempts - total_attempts
```

---
## 🔄 Indentação Correta
A indentacão é **obrigatória** no Python para blocos de código como loops, condições e funções. O PEP 8 recomenda **4 espaços por nível** de indentacão.

Exemplo:
```python
count = 0
login_status = True

while login_status:
    print("Tente novamente.")
    count += 1
    
    if count == 4:
        login_status = False
```

---
## ⚠️ Erros Comuns de Sintaxe
Os erros de sintaxe podem impedir que seu código seja executado corretamente. Aqui estão algumas boas práticas:

### 🔒 Tipos de Dados
- Strings devem estar **entre aspas**: `username = "bmoreno"`
- Números **não precisam de aspas**: `login_attempts = 5`
- Listas devem estar **entre colchetes** e separadas por vírgulas: `users = ["bmoreno", "tshah"]`

### 🔠 Uso de Dois-Pontos
Cabeçalhos de funções, loops e condições devem sempre terminar com **dois-pontos (:).**

Exemplo:
```python
def remaining_login_attempts(maximum_attempts, total_attempts):
    return maximum_attempts - total_attempts
```

---
## 🔗 Recursos Adicionais
Para melhorar suas práticas de programação em Python, consulte o guia oficial:
- 🔍 **[PEP 8 - Guia de estilo para Python](https://peps.python.org/pep-0008/)**

---
## 🌟 Conclusão
- Siga as **diretrizes do PEP 8** para melhor legibilidade.
- Use **comentários** para explicar seu código.
- **Indentacão correta** é essencial para a execução do código.
- Fique atento aos **erros comuns de sintaxe** para evitar falhas.

Dúvidas ou sugestões? ✌️ Comente e contribua!

---
💪 **Mantenha seu código limpo e legível!** 💪

