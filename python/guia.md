# 📌 Guia de Expressões Regulares no Python

![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
![RegEx](https://img.shields.io/badge/RegEx-Expressions-red)

## 🔍 O que são Expressões Regulares?
Uma **expressão regular (RegEx)** é uma sequência de caracteres que forma um padrão. No Python, elas são usadas para buscar padrões específicos, como **endereços IP, e-mails e IDs de dispositivos**.

Para utilizar expressões regulares no Python, primeiro importe o módulo `re`:

```python
import re
```

## 🛠 Uso da função `re.findall()`
A função `re.findall()` retorna todas as correspondências de um padrão dentro de uma string.

**Exemplo:**
```python
import re
resultado = re.findall("ts", "tsnow, tshah, bmoreno")
print(resultado)
```
📌 **Saída:** `['ts', 'ts']`

## ✨ Principais Símbolos de Expressões Regulares

### 🔡 Símbolos para Tipos de Caracteres
| Símbolo | Descrição |
|---------|-----------|
| `.` | Corresponde a qualquer caractere (incluindo símbolos) |
| `\w` | Corresponde a qualquer caractere alfanumérico (`a-z`, `A-Z`, `0-9`, `_`) |
| `\d` | Corresponde a qualquer dígito (`0-9`) |
| `\s` | Corresponde a qualquer espaço em branco |
| `\.` | Corresponde ao caractere de ponto final (`.`) |

**Exemplo:**
```python
import re
resultado = re.findall("\d", "h32rb17")
print(resultado)
```
📌 **Saída:** `['3', '2', '1', '7']`

### 🔢 Símbolos para Quantificar Ocorrências
| Símbolo | Descrição |
|---------|-----------|
| `+` | Uma ou mais ocorrências do caractere anterior |
| `*` | Zero ou mais ocorrências do caractere anterior |
| `{n}` | Exatamente `n` ocorrências do caractere anterior |
| `{n,m}` | Entre `n` e `m` ocorrências do caractere anterior |

**Exemplo:** Encontrar grupos de um ou mais dígitos.
```python
import re
resultado = re.findall("\d+", "h32rb17")
print(resultado)
```
📌 **Saída:** `['32', '17']`

## 🏗 Construindo um Padrão
Para construir um padrão, divida a busca em partes menores.

### **Exemplo: Extraindo nomes de usuário e tentativas de login**
**Dados:**
```python
employee_logins_string = "1001 bmoreno: 12 Marketing 1002 tshah: 7 Human Resources 1003 sgilmore: 5 Finance"
```
**Padrão:**
```python
import re
pattern = "\w+:\s\d+"
resultado = re.findall(pattern, employee_logins_string)
print(resultado)
```
📌 **Saída:** `['bmoreno: 12', 'tshah: 7', 'sgilmore: 5']`

## 🎯 Principais Lições
✅ Expressões regulares são úteis para **buscar padrões** em strings.  
✅ O módulo `re` fornece várias funções, como `re.findall()`, para buscar padrões.  
✅ Símbolos como `\d`, `\w`, `+`, `*` ajudam a definir padrões mais flexíveis.  

🚀 **Teste e refine suas expressões para obter os melhores resultados!**
