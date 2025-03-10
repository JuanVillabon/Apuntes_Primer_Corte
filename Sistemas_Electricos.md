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
