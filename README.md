# Exemplos de Operações com Matrizes em NumPy

## Descrição

Este documento consolida **todos os exemplos de manipulação de matrizes enviados**, utilizando a biblioteca **NumPy**. Os trechos demonstram operações essenciais em computação numérica e álgebra linear.

---

## Código Consolidado

```python
import numpy as np
import matplotlib.pyplot as plt

# ================= MATRIZ 1 — Criação e Multiplicação Escalar =================

A = np.array([1, 2, 3, 4]).reshape(2, 2)
A = 3 * A

print("Matriz A (multiplicada por 3):")
print(A)

# ================= MATRIZ 2 — Valores Aleatórios =================

a = np.random.rand(60)

print("\nValores aleatórios:")
print(a)

plt.hist(a, bins=10, edgecolor='black')
plt.xlabel("Valor")
plt.ylabel("Frequência")
plt.title("Histograma")
plt.show()

print("\nFormato após ravel():")
print(a.ravel().shape)

# ================= MATRIZ 3 — Matriz Diagonal =================

Diag = np.diag([1, 2, 3, 4, 5])

print("\nMatriz Diagonal:")
print(Diag)

# ================= MATRIZ 4 — Matriz Identidade =================

identidade = np.eye(5, 5)

print("\nMatriz Identidade:")
print(identidade)

# ================= MATRIZ 5 — Matriz de Zeros =================

zeros = np.zeros([3, 3])

print("\nMatriz de Zeros:")
print(zeros)

# ================= MATRIZ 6 — Multiplicação Vetorial =================

v1 = np.array([1.0, 2.0, 3.0])
v2 = np.array([2.0, 2.0, 2.0])

print("\nMultiplicação elemento a elemento:")
print(v1 * v2)
