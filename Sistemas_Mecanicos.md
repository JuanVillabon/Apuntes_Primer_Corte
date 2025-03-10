# Apuntes Primer Corte
## Que es un sistema
Un sistema es un conjunto de elementos interrelacionados que trabajan en conjunto para cumplir una función específica. En ingeniería, los sistemas pueden ser mecánicos, eléctricos, hidráulicos, neumático, térmico y combinaciones, en donde tendremos una entrada específica y una salida.

### Principio general del modelamiento
El principio general de modelamiento se basa en la conservación de la masa o la energía dentro de un sistema, estableciendo que la tasa de acumulación de una magnitud es igual a la diferencia entre su flujo de entrada y su flujo de salida. Esto significa que la cantidad de masa o energía en un sistema cambia en función de lo que ingresa y lo que sale.

$$ Tasa de acumulación \frac{Masa}{Energia} = Flujo \frac{Masa}{Energia} Entrada - Flujo  de \frac{Masa}{Energia} Salida $$

## 1. Sistemas Mecanicos
Un sistema mecánico es un conjunto de elementos físicos interconectados que interactúan mediante fuerzas y movimientos para realizar una función específica. Estos sistemas pueden estar compuestos por componentes como engranajes, palancas, resortes, masas, amortiguadores y mecanismos de transmisión de movimiento.

### 1.1. Sistemas Masa - Resorte - Amortiguador
El sistema masa-resorte-amortiguador es un modelo fundamental en control o dinamica de sistemas mecánicos y se utiliza para describir el comportamiento de estructuras sometidas a vibraciones. Este sistema consta de tres elementos principales:

- Masa (m): Es el objeto que se mueve, puede ser cualquier cosa con peso, como un bloque, un coche o una persona en un columpio.

- Resorte (k): Es un elemento que almacena y libera energía. Cuando se estira o comprime, intenta volver a su posición original. Cuanto más rígido sea, más fuerte será la fuerza que ejerce.

- Amortiguador (c): Es un componente que reduce el movimiento al disipar energía. Funciona como un freno que impide que el sistema siga oscilando demasiado tiempo.

![Captura de pantalla 2024-09-18 002051](https://github.com/user-attachments/assets/a776c23b-8b11-439d-ab1c-3a530646ce1d)

- $F_{R} = k_{2} * X →  Ley de Hooke$

- $F_{F} = k_{1} * V_{m} →  Fricción viscosa$

- $F = m * a →  Leyes de Newton$

### 1.2. Modelamiento en sistemas mecanicos
## Diagramas de cuerpo libre
Un diagrama que muestra las fuerzas que actúan sobre el objeto. El objeto se representa mediante un punto con fuerzas dibujadas como flechas que apuntan en dirección opuesta al punto. A veces llamado diagrama de fuerza.

#### Ejemplo:

![Captura de pantalla 2024-09-18 002051](https://github.com/user-attachments/assets/a776c23b-8b11-439d-ab1c-3a530646ce1d)

Diagrama de cuerpo libre:

![Captura de pantalla 2024-09-18 003035](https://github.com/user-attachments/assets/b2e0302b-e8fa-4a45-a797-2e0f6d824ab8)

$$ u - F_{R} - F_{F} = m * a $$

## Ejercicios

