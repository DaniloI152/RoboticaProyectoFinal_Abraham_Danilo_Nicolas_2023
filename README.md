# Proyecto Final Robótica
### Integrantes: 
- Danilo Enrique Insuasty Delgado.
- Abraham Másmela Ramirez.
- Nicolás Prieto Solano.


## Objetivos:
• Desarrollo de un sistema robotizado para la automatización del proceso de Pick & Place y alistamiento de pedidos

## Consideraciones:
• El proceso de alistamiento: Se debe tomar el contenedor (balde) del extremo de la banda transportadora y
ubicarlo en un lugar de alistamiento. Se deben tomar 3 piezas distintas de la estantería de madera y ubicarlas
en el balde. El pedido listo (balde+piezas) debe ser ubicado de regreso sobre la banda transportadora. <br>
• Alistamiento de la estantería: La estantería de madera tiene 6 posiciones (A,B,C,D,E,F), se deben ubicar
6 piezas distintas en cada posición de la estantería. El tamaño, forma, material y demás características pueden
ser ajustadas de acuerdo a la herramienta diseñada.<br>
• Posicionamiento de los elementos: Tanto la estantería como las piezas en cada una de las 6 posiciones
pueden ser posicionadas al espacio de trabajo diestro del manipulador, todo ajuste se debe realizar con el
brazo inmóvil y solamente al inicio del proceso.<br>
• Análisis de tiempo manual: Se debe realizar pruebas de trabajo manual utilizando una sola mano, donde
se pueda identificar el tiempo promedio de alistamiento manual para las combinaciones estudiadas. <br>

## Diseño de la herramienta y modelos 3D:
En el diseño de la herramienta, se tomaron en cuenta las dimensiones de las piezas, el balde, la ventosa y el estante, para permitir la ejecución de las rutinas de manera eficiente. Se utilizó el software Inventor para modelar la herramienta y se consideró la opción de fabricarla mediante impresión 3D. Sin embargo, se determinó que para obtener una pieza más resistente y de mayor facilidad de construcción, se utilizarían láminas de MDF de 10mm cortadas con láser. Además, se realizaron cortes en las piezas que se colocarían en el estante utilizando diferentes formas geométricas. 

<div>
<p style = 'text-align:center;' align="center">
<img src="https://github.com/DaniloI152/RoboticaProyectoFinal_Abraham_Danilo_Nicolas_2023/blob/main/Herramienta/porta.png" width="600px" >
</p>
</div>

[Planos de corte de las piezas](https://github.com/DaniloI152/RoboticaProyectoFinal_Abraham_Danilo_Nicolas_2023/blob/main/Herramienta/Piezas2.pdf)
[Planos de corte de Herramienta](https://github.com/DaniloI152/RoboticaProyectoFinal_Abraham_Danilo_Nicolas_2023/blob/main/Herramienta/plano%20corte.pdf)

Se realizó el modelado del gancho y la ventosa para incorporarlos en la simulación del sistema. Para el gancho, se compró uno y se modelo con sus respectivas dimeniones. En el caso de la ventosa, se tuvieron en cuenta las dimensiones principales, como el diámetro y la altura, y se modeló como un cilindro. Además, se consideraron las dimensiones de las demás piezas, que tienen un grosor de 10 mm. Estas dimensiones se agregaron a la altura de la ventosa para simplificar la colocación de los modelos 3D en la simulación, al incluir esta dimensión adicional en la ventosa, se aseguró que la pieza estuviera presente en todo momento, lo que permitió verificar que las trayectorias se realizaran sin colisiones. Esta aproximación facilitó el análisis y la validación del sistema en la simulación. <br>

Para el modelado de la banda se tomaron sus dimensiones de altura, ancho y largo y se reprensetó como un prisma rectangular 

<div>
<p style = 'text-align:center;' align="center">
<img src="https://github.com/DaniloI152/RoboticaProyectoFinal_Abraham_Danilo_Nicolas_2023/blob/main/Herramienta/Banda.png" width="600px" >
</p>
</div>
[Planos de la banda](https://github.com/DaniloI152/RoboticaProyectoFinal_Abraham_Danilo_Nicolas_2023/blob/main/Herramienta/Banda.pdf)

Se procedio a hacer lo mismo con el estante donde irán posicionadas las piezas

<div>
<p style = 'text-align:center;' align="center">
<img src="https://github.com/DaniloI152/RoboticaProyectoFinal_Abraham_Danilo_Nicolas_2023/blob/main/Herramienta/estante.png" width="600px" >
</p>
</div>
[Planos de la banda](https://github.com/DaniloI152/RoboticaProyectoFinal_Abraham_Danilo_Nicolas_2023/blob/main/Herramienta/estante.pdf)

## Robot Studio

### Simulación
### Código

## Resultados

## Análisis de tiempos

### Proceso manual
### Proceso automático con el robot

## Conclusiones
• El modelado completo del espacio de trabajo es crucial para el éxito del desarrollo del proyecto. Aunque se crean planos que indican la ubicación de los elementos y se generan modelos en 3D con dimensiones precisas, al probar las rutinas nos encontramos con la situación de que las piezas habían sido cambiadas de posición, lo que requería actualizar las posiciones. Para abordar este problema de manera sencilla, se estableció una vinculación entre cada punto de las trayectorias y las piezas correspondientes. De esta forma, al mover la pieza a su ubicación correcta, las trayectorias se ajustaban automáticamente en consecuencia.
