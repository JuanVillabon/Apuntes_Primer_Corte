# Sistemas Electricos

Un sistema eléctrico es un conjunto de componentes y dispositivos diseñados para la generación, transmisión, distribución y utilización de la energía eléctrica de manera eficiente y segura. Estos sistemas son fundamentales en la vida cotidiana e industrial, ya que permiten la operación de máquinas, iluminación, telecomunicaciones y otros servicios esenciales.

## Circuito RLC

- *Resistencia:* se le denomina resistencia a la oposición al flujo de corriente eléctrica a través de un conductor. La unidad de resistencia en el Sistema Internacional es el ohmio, que se representa con la letra griega Ω.

![image](https://github.com/user-attachments/assets/5aa07a3d-6455-4dfb-8036-21d9370bd5bc)
Ley de Ohm
$$ R = \frac{v(t)}{i(t)} $$

- *Condensador:* Un condensador es un dispositivo capaz de almacenar energía en forma de campo eléctrico. Está formado por dos armaduras metálicas paralelas, generalmente de aluminio separadas por un material dieléctrico.

![image](https://github.com/user-attachments/assets/780cec15-5602-4c4a-a00f-fb38ba603d00)
Carga de un condensador
$$ i(t) = C \frac{dv(t)}{dt} $$

- *Inductor:* Un inductor es un componente pasivo utilizado en la electrónica que tiene la capacidad de almacenar energía en un campo magnético creado por una corriente eléctrica que pasa a través de él. Este dispositivo tiene la particularidad de oponerse a los cambios de corriente en un circuito, fenómeno conocido como inductancia.

![image](https://github.com/user-attachments/assets/08798599-866f-4d92-92d6-d28b880ef77a)
Carga de un Inductor
$$ v(t) = L \frac{di(t)}{dt} $$

- *Ejemplo con ley de Kirchoff*

![image](https://github.com/user-attachments/assets/fec43beb-dfe9-41d8-a6ae-eb1c5e5246e0)

~ Aplicando ley de Kirchoff ~
$$ - u + V_{R} + V_{L} + V_{C} = 0 $$

$$ - u(t) + i(t) * R + L \frac{di(t)}{dt} + y(t) = 0 $$

~ Aún no etsá en términos de la variable Y ~

$$ - u(t) + C \frac{dy(t)}{dt} * R + L \frac{d}{dt} (C \frac{dt(t)}{dt}) + y(t) = 0 $$

- $i(t) = C \frac{dy(t)}{dt}$

$$ -u(t) + RC \frac{dy(t)}{dt} + LC \frac{d^{2}y(t)}{dt^{t}} + y(t) = 0 $$

## Nodos

Un nodo es la conexión que se genera entre dos o más ramas. Ese punto de conexión puede estar formado por la conexión de los elementos, y también puede formarse por un corto circuito, es decir, un alambre de conexión.

- *Ejemplo aplicando Nodos*

![image](https://github.com/user-attachments/assets/2c34be11-285b-4d22-aacc-0e2c4e6e47d9)

Aplicando ley de kirchoff de corrientes LKC

$$ i_{u} - i_{1} - i_{c} = 0 $$

$$ i_{u}(t) - \frac{V_{AB}}{0,5} - 2 \frac{dy(t)}{dt} = 0 $$

$$ V_{AB} = i_{c} * 1 + y(t) $$

$$ V_{AB} = 2 \frac{dy(t)}{{dt} + y(t) $$

$$ u(t) - \frac{2}{0,5} \frac{dy(t)}{dt} - \frac{1}{0,5} y(t) - 2 \frac{dy(t)}{dt} = 0 $$

$$ u(t) - 6 \frac{dy(t)}{dt} - 2y(t) = 0 $$


# Circuitos con amplificadores operacionales

## Amplificador no inversor

Un amplificador no inversor es un circuito basado en un amplificador operacional (Op-Amp) que amplifica una señal de entrada sin invertir su fase. Es decir, la señal de salida tiene la misma fase que la señal de entrada.

- *Ventajas*
- Alta impedancia de entrada (ideal para sensores y señales débiles).
- No invierte la fase de la señal.
- Fácil de ajustar la ganancia con solo cambiar Rf y R1

![image](https://github.com/user-attachments/assets/4f6dc34c-3853-4849-b80d-53a325dee49f)

- *Caracteristicas*
- Las tension en ambas entradas del amplificador son iguales V+ = V-.
- La corriente a las entradas del amplificador es 0.
- La impedancia de entrada es muy grande
- La impedancia de salida es muy pequeña

- *Ejemplo*

![image](https://github.com/user-attachments/assets/ba8a06fd-949c-408d-970e-39d30e650549)

$$ i_{1} - i_{2} = 0 $$

$$ \frac{e_{0} - e_{i}}{R_{2}} - \frac{e_{i}}{R_{1}} = 0 $$

$$ \frac{e_{0}}{R_{2}} = e_{i} (\frac{1}{R_{2}} + \frac{1}{R_{1}}) $$

$$ e_{o} = e_{i} (1 + \frac{R_{2}}{R_{1}}) $$
