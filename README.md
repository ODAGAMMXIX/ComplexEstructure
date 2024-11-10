# ComplexEstructure
Complexidade de Algoritmos de Ordenação - Estrutura de Dados
online Python interpreter https://www.tutorialspoint.com/execute_matplotlib_online.php

![Gráfico de Complexidade - Algoritmos de Ordenação ](https://github.com/ODAGAMMXIX/ComplexEstructure/blob/main/DEV-ORDENACAO-COMPLEXIDADE.jpg)


import matplotlib.pyplot as plt
import numpy as np

# Número de elementos
n = np.linspace(1, 100, 100)

# Complexidades
o_1 = np.ones_like(n)
o_log_n = np.log2(n)
o_n = n
o_n_log_n = n * np.log2(n)
o_n2 = n**2

# Criando o gráfico
plt.figure(figsize=(10, 6))
plt.plot(n, o_1, label='O(1)')
plt.plot(n, o_log_n, label='O(log n)')
plt.plot(n, o_n, label='O(n)')
plt.plot(n, o_n_log_n, label='O(n log n)')
plt.plot(n, o_n2, label='O(n^2)')

# Adicionando títulos e legendas
plt.title('Complexidades de Algoritmos')
plt.xlabel('Número de Elementos (n)')
plt.ylabel('Tempo de Execução')
plt.yscale('log')  # Escala logarítmica para melhor visualização
plt.legend()
plt.grid(True)
plt.show()
