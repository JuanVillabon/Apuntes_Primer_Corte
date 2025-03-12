# Sistemas Termicos

Un sistema térmico es un sistema que intercambia, genera o almacena energía en forma de calor. Su funcionamiento se basa en los principios de la termodinámica, incluyendo la transferencia de calor, el trabajo y la energía interna.

![image](https://github.com/user-attachments/assets/ae492117-1688-4b47-9292-958c3c525507)

El sistema mostrado es un tanque térmico de calentamiento donde un líquido frío ingresa, es mezclado por un agitador y calentado mediante un calentador interno. La agitación asegura una temperatura uniforme en el fluido mientras el calentador transfiere energía térmica, elevando su temperatura. Una vez calentado, el líquido sale del sistema para su uso en procesos industriales, alimentarios o de calefacción.

- *Formulas*

$$ R = \frac{\theta}{h_{o}} $$

$$ Cd\theta = (h_{i} - h_{o})dt $$

$$ C \frac{d \theta}{dt} = h_{i} - h_{o} $$

$$ RC \frac{d\theta}{dt} + \theta = Rh_{i} $$

# Potenciómetro

Un potenciómetro es un resistor variable que se usa para ajustar el voltaje en un circuito eléctrico. Tiene tres terminales: dos están conectados a los extremos de una resistencia fija y el tercero a un contacto deslizante (cursor), que varía la resistencia efectiva al moverse.

### Potenciómetro de rotación 

Un potenciómetro de rotación es un tipo de potenciómetro en el que la resistencia se ajusta girando un eje o perilla. A medida que el eje rota, un contacto deslizante (cursor) se mueve sobre una pista resistiva, variando la resistencia y permitiendo el control del voltaje de salida.

![image](https://github.com/user-attachments/assets/742a3221-3de5-4fd8-830e-df9befac170e)

$$ V_{o} = \frac{\theta}{\theta_{máx}} V_{cc} $$

### Potenciómetro de translación 

Un potenciómetro de traslación (o potenciómetro lineal) es un tipo de potenciómetro en el que la resistencia se ajusta mediante un movimiento lineal en lugar de rotación. Funciona con un cursor que se desliza sobre una pista resistiva al mover una varilla o una guía, modificando la resistencia y permitiendo el control del voltaje de salida.

![image](https://github.com/user-attachments/assets/b85a17eb-5a10-499c-8968-078dfc1b928c)

$$ V_{o} = \frac{x}{x_{máx}} V_{cc} $$

# Tacómetros

Un tacogenerador es un dispositivo electromecánico que convierte la velocidad de rotación de un eje en una señal eléctrica, típicamente un voltaje proporcional a dicha velocidad. Se utiliza comúnmente para medir y controlar la velocidad en sistemas industriales y de automatización.

![image](https://github.com/user-attachments/assets/df1d4215-5743-48dc-b5a2-84cd6d371fb6)

$$ V(t) = k \frac{d/theta(t)}{dt} $$

# Sensores transmisores

Los sensores transmisores son dispositivos que integran la función de detección de una variable física (como temperatura, presión o nivel) y la capacidad de transmitir esa información en forma de una señal estándar, generalmente una corriente de 4-20 mA o una señal digital. Esta integración permite una comunicación eficiente y precisa en sistemas de monitoreo y control industrial.

### Lineales

Un sensor lineal es aquel cuya salida es directamente proporcional a la magnitud de la variable que mide. Esta proporcionalidad implica que la función de transferencia del sensor es una línea recta, facilitando la interpretación y procesamiento de la señal.

$$ TO = PV * K $$

### No lineales

Un sensor no lineal es aquel cuya salida no guarda una relación directa y proporcional con la variable medida. La función de transferencia de estos sensores es una curva, lo que puede complicar la interpretación de la señal y requerir métodos adicionales para su correcta utilización.

$$ a * \frac{d(TO)}{dt} + b * TO = PV $$



