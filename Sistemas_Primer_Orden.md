# Sistemas de primer orden

## Transformada de Laplace

El método de la transformada de Laplace es una herramienta operacional útil para resolver ecuaciones diferenciales lineales con coeficientes constantes. Utilizada para convertir funciones del dominio del tiempo en funciones del dominio de la frecuencia. Es especialmente útil en el análisis y diseño de sistemas lineales, así como en la resolución de ecuaciones diferenciales. Esto permite que la solución de la ecuación diferencial se obtenga mediante tablas de transformadas de Laplace o utilizando la técnica de fracciones parciales.

- *Transformada de una función*

$$ L[f(t)] = F(s) $$

- *Transformada de la derivada*

$$ L[f'(t)] = _{s}F(s) - f(0) $$

$$ L[f''(t)] = _{s^{2}}F(s) - _{s}f(0) - f'(0) $$

$$ L[f^{n}(t)] = _{s^{n}F(s)} - s^{(n-1)}f(0) - ... - sf^{(n-1)}(0) - f^{n}(0) $$

- *Transformada de la integral*

$$ L[\int f(t)dt ] = \frac{1}{s} F(s) $$

## Funcón de transferencia 

Una función de transferencia es una representación matemática de la relación entre la entrada y la salida de un sistema dinámico en el dominio de la frecuencia (generalmente usando la variable 𝑠 en el espacio de Laplace). Se usa en ingeniería de control y sistemas para analizar y diseñar respuestas a diferentes señales de entrada.

$$ Se despeja \frac{salida}{entrada} es decir: \frac{Y(s)}{U(s)} $$

Todas las condiciones iniciales de la ecuación diferencial son iguales a 0

- *Nota:* Esto sólo alica cuandose van a hacer funciones de transferencia, en el caso de querer solucionar la ecuacion diferencial si son necesarioas las condiciones iniciales y no necesariamente son 0

- *Ejemplo*

Hallar la función de transferencia para la siguiente ecuación diferencial:

$$ \ddot{y}(t) + 3\dot{y}(t) + 2y(t) = 2\dot{u}(t) - u(t) $$

Aplicando transformada de LaPlace

$$ s^{2}Y(s) - sy(0) - sy'(0) + 3(sY(s) - y(0)) + 2Y(s) = 3(sU(s) - u(0)) - U(s) $$

Despejando salida / entrada

$$ \frac{Y(s)}{U(s)} = \frac{3s-1}{s^{2}+3s+2} + \frac{(s+3)y(0)+y(0)-3u(0)}{s^{2}+3s+2} $$

### Hallar los zeros de una función de transferencia

$$ G(s) = \frac{Y(s)}{U(s)} = \frac{3s-1}{s^{2}+3s+2} = \frac{N(s)}{D(s)} $$

- N(s) = 0
- 3s - 1 = 0

$$ s = \frac{1}{3} $$

![image](https://github.com/user-attachments/assets/3e02d7bd-fb24-46e0-9108-24b0a0b7ea7d)

### Hallar los polo de una función de transferencia

$$ G(s) = \frac{Y(s)}{U(s)} = \frac{3s-1}{s^{2}+3s+2} = \frac{N(s)}{D(s)} $$

- D(s) = 0
- $s^{2}+3s+2=0$

$$ (s + 1)(s + 2) = 0 $$

- S = -1

- s = -2

![image](https://github.com/user-attachments/assets/8d21627d-ff49-46eb-8b02-6ec858e3a2c5)

## Entradas de prueba a un sistema

### Entrada Escalón

Una entrada escalón (o escalón unitario) es una señal de entrada comúnmente utilizada en el análisis de sistemas de control. Se representa como una función que cambia abruptamente de 0 a 1 en t = 0 y se mantiene constante en 1 para t≥0. Matemáticamente, se expresa como:

$$ u(t) = [A para t > t_{o} , 0 para t < t_{o} $$

$$ L[u(t)] = \frac{A}{s} $$

![image](https://github.com/user-attachments/assets/091be5b1-330e-49f1-bb26-b556215b4d2f)

### Entrada Rampa

Una entrada rampa es una señal que aumenta linealmente con el tiempo y se usa comúnmente en el análisis de sistemas de control para evaluar la capacidad de seguimiento de un sistema ante cambios progresivos en la entrada. Matemáticamente, se define como:

$$ x(t) = [ At para t > t_{o} , 0 para t < t_{o} $$

$$ L[x(t)] = \frac{A}{s^{2}} $$

![image](https://github.com/user-attachments/assets/2754c524-60ad-4be0-9780-afb868f962cf)

### Entrada Parábola

Una entrada parábola es una señal de entrada que crece cuadráticamente con el tiempo y se usa en análisis de sistemas de control para evaluar el rendimiento del sistema frente a variaciones aceleradas. Matemáticamente, se define como:

$$ r(t) = [At^{2} para t > t_{o} , 0 para t < t_{o} $$

$$ L[r(t)] = \frac{A}{s^{3}} $$

![image](https://github.com/user-attachments/assets/a0e3997c-f727-4c29-acf4-5c364969f922)


## Sistemas de primer orden

Los sistemas de primer orden son sistemas dinámicos cuya ecuación diferencial tiene una derivada de primer orden como la de mayor grado. Se caracterizan por tener una función de transferencia de la forma:

$$ \frac{Y(s)}{U(s)} = \frac{c}{as + b} $$

- *Ejemplo*

![image](https://github.com/user-attachments/assets/f8c18c41-d957-475a-a143-ae1025667397)

$$ \frac{Y(s)}{U(s)} = \frac{c}{as + b} $$

- a = R1A1
- b = 1
- c = R1

$$ R_{1}A_{1} \frac{dh_{1}}{dt} = R_{1}q_{i} - h_{1} $$

$$ \frac{H_{1}(s)}{Q_{i}(s)} = \frac{R_{1}}{R_{1}A_{1}s+1} $$

### Fomra canónica de los sistemas de primer orden

La forma canónica de un sistema de primer orden permite analizar sus características esenciales como la rapidez de respuesta, estabilidad y precisión ante diferentes señales de entrada. Entre las aplicaciones más comunes de estos sistemas se encuentran los circuitos eléctricos RC, los sistemas térmicos, los sistemas hidráulicos y los procesos industriales con dinámica lenta.

$$ \frac{Y(s)}{U(s)} = \frac{c}{as + b} $$

$$ \frac{Y(s)}{U(s)} = \frac{\frac{c}{b}}{\frac{a}{b}s+1} $$

- La forma canónica considera:

$$ G(s) = \frac{K}{𝜏s + 1} $$

donde:

- K es la ganancia estática (define la respuesta final del sistema).

- 𝜏 es la constante de tiempo (indica la rapidez con la que el sistema responde a una entrada).

- s es la variable en el dominio de Laplace.

$𝜏=\frac{a}{b}$ Constante de tiempo

$K=\frac{c}{b}$ Ganancia estática

- *Ejemplo*

Identificar el 𝜏 y K para el siguiente sistema:

$$ \frac{Y(s)}{U(s)} = \frac{0,8}{s + 1} $$

por lo tanto 𝜏 = 1 y K = 0,8

### Ejercicios

1. Dada la siguiente función de transferencia, encuentra la constante de tiempo y la ganancia estática

$$ G(s) = \frac{10}{4s + 20} $$

- Factorizamos el coeficiente

$$ G(s) = \frac{10}{4(s + 5)} $$

- Constante de tiempo = $\frac{1}{5}$

- Ganancia estática = $\frac{10}{20} -> \frac{1}{2}$ 

2. Dada la siguiente función de transferencia, encuentra la constante de tiempo y la ganancia estática

$$ G(s) = \frac{8}{5s + 4} $$

Contante de tiempo = $\frac{5}{4}$

Ganancia estática = $\frac{8}{4} -> 2$

## Respuesra temporal de un Sistema de primer orden

### Respuesta de una entrada escalón

![image](https://github.com/user-attachments/assets/a1af55be-8a8a-44d5-87e9-001f87bd4643)

constante de tiempo del sistema

![image](https://github.com/user-attachments/assets/d718d448-5865-4f6e-aaf6-7f6d1e0bc327)

- $$ y(t) = AK(1 - e^{-\frac{t}{𝜏}}) $$

![image](https://github.com/user-attachments/assets/f7927a71-7560-4cf0-8e17-5f7707020a59)

### Respuesta de una entrada rampa

$$ Y(s) = \frac{AK}{s^{2}(𝜏s + 1)} $$

Fracciones parciales

$$ Y(s) = AK (\frac{1}{s^{2}} - \frac{1𝜏}{s} + \frac{𝜏^{2}}{𝜏s + 1}) $$

$$ L^{-1} [Y(s)] = y(t) = AK(t - 𝜏 + 𝜏e^{-\frac{t}{𝜏}}) $$

![image](https://github.com/user-attachments/assets/317e0c4d-5343-413b-ba0b-12f7f876dbb5)

Constante de tiempo del sistema

![image](https://github.com/user-attachments/assets/9fee4655-02fb-4e0f-bef6-c19aeb949a2d)

$$ m = \frac{4𝜏AK - 3𝜏AK}{5𝜏 - 4𝜏} = AK $$

![image](https://github.com/user-attachments/assets/27f0abb5-53b6-4323-a2d1-b497af4901c1)

### Respueta de una entrada al impulso

![image](https://github.com/user-attachments/assets/c21a23f6-9b44-472d-adc0-85814e4557e8)

$$ y(t) = \frac{AK}{𝜏} e^{-\frac{t}{𝜏} $$

