# 📜 Listas em Python para Segurança Cibernética

![Python](https://img.shields.io/badge/Python-3.9%2B-blue?style=for-the-badge&logo=python)  
![Cybersecurity](https://img.shields.io/badge/Cybersecurity-%F0%9F%94%92-important?style=for-the-badge)

As listas são uma das estruturas de dados mais usadas em Python. Como Analista de Segurança, você pode usá-las para armazenar nomes de usuários, endereços IP, logs de eventos e muito mais!

## 🔹 O que são listas?
Uma lista em Python é uma estrutura de dados que pode conter vários tipos de elementos. Ela é mutável, ou seja, pode ser alterada após sua criação.

```python
# Exemplo de lista com usernames
usernames = ["elarson", "fgarcia", "tshah", "sgilmore"]
print(usernames)
```

## 🔍 Acessando elementos
Podemos acessar elementos da lista utilizando a indexação:

```python
print(usernames[2])  # Saída: tshah
```

🔸 **Importante**: A indexação em Python começa do `0`.

## ✂ Extraindo partes da lista (slicing)
Podemos pegar partes da lista usando `:`:

```python
print(usernames[0:2])  # Saída: ['elarson', 'fgarcia']
```

## 🔄 Alterando elementos da lista
```python
usernames[1] = "bmoreno"
print(usernames)  # Saída: ['elarson', 'bmoreno', 'tshah', 'sgilmore']
```

## ⚙ Métodos úteis para listas

### 📌 Inserindo elementos: `.insert()`
Adiciona um elemento em uma posição específica:

```python
usernames.insert(2, "wjaffrey")
print(usernames)
```

### ❌ Removendo elementos: `.remove()`
Remove a **primeira ocorrência** do elemento na lista:

```python
usernames.remove("elarson")
print(usernames)
```

### ➕ Adicionando ao final: `.append()`
Adiciona um elemento ao **final** da lista:

```python
usernames.append("btang")
print(usernames)
```

### 🔎 Encontrando índices: `.index()`
Retorna a posição do elemento na lista:

```python
index = usernames.index("tshah")
print(index)  # Saída: 2
```

## 🏁 Conclusão
As listas são ferramentas poderosas e essenciais para qualquer Analista de Segurança. Você pode utilizá-las para armazenar e manipular dados de forma eficiente!

---
💻 *Criado por [SeuNome](https://github.com/seuusuario)* | 🚀 Siga para mais conteúdos!
