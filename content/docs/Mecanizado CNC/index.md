---
title: '2. Mecanizado CNC'
date: 2020-06-17T19:30:08+10:00
draft: false
weight: 7
summary: 

-------

En esta sección de mecanizado CNC, explicaré cual es el funcionamiento de esta maquina, entregaré un link para descargar su manual de uso y finalmente mostraré un video paso a paso de como hacer que un objeto 3d (en este caso la silla Fresia) se pueda configurar en Fusion 360 para que luego sea cortada.



### 1) Router CNC

![cnc](/img/cnc/1.png)

El router CNC es una cortadora automatizada, impulsada por motores que funcionan gracias a un sistema de control numérico. Estas máquinas permiten realizar cortes de manera precisa de 2 y hasta 3 dimensiones.

Son muy útiles en la realización de trabajos en serie, puesto que pueden cortar piezas idénticas y en gran volumen en plazos más cortos que si utilizara una máquina de corte convencional. Lo que permite a tu negocio alcanzar mayor productividad

Las máquinas CNC son compatibles con diferentes materiales blandos, puede cortar maderas, PVC, triplay, poliuretano, acrílico y algunos metales no ferrosos como el aluminio, latón y el bronce, entre muchos otros.

Gracias a su sistema de control numérico, los Routers CNC son muy útiles para fabricar muebles, cortar materiales y tallar maderas. Pues la precisión de sus cortes acelera el proceso de producción y reduce los residuos, por lo que vuelve a tu negocio más productivo y eficiente.

Las máquinas CNC no necesitan descansar, únicamente necesitan detenerse cuando requieren mantenimiento o reparación, lo que aumenta la capacidad de producción; además de que no se requiere de mucho capital humano, puesto que una persona es capaz de supervisar una o varias máquinas CNC sin mayor problema.



![cnc](/img/cnc/3.jpg) Tallada en Router CNC

---

### 2) Manual de uso

Para maquina Router CNC 1212

{{< boton-descargar src="paso_a_paso_router.pdf" >}} 

**Haz click en el casillero.**

---

### 3) Silla Fresia 

{{< iframe-fusion2 >}}

---

{{< boton-descargar src="silla_fresia.f3d" >}}

**Haz click en el casillero.**

**Paso 1**:
Descargar archivo en el casillero y abrir archivo en Fusion 360.

**Paso 2**:
Crear un sketch rectangular de 1220x1220 mm y extruir 15 mm.

**Paso 3**: 
Copiar cada una de las partes de la silla y llevarlas al plano XY de manera que queden en el mismo sentido de la plancha.

**Paso 4**:
Mover cada una de las partes a la plancha y utilizar bien los espacios, asegurandose que cada uno de los elementos quede dentro de la plancha.

**Paso 5**:
Cambiamos de DESIGN a MANUFACTURE y creamos un setup. Aqui elegimos la maquina (Autodesk Generic 3-axis), se elije el tipo de operacion "milling" y le damos una orientacion "select Z axis/plane & x axis", orientando nuestro eje x y el punto de origen. Luego definimos el stock "from solid", seleccionamos la plancha que dibujamos y seleccionamos las piezas a cortar.

**Paso 6**: Creamos un 2d countour, seleccionando las partes huecas inferiores de la figura. Aqui se debe elegir la fresa que vamos a utilizar, en este caso particular utilizaremos una "flat end mill de 0 mm x 6mm x 20mm x 63mm". Finalmente en la sección "Passes" en Multiple depths cambiamos el maximo a 3mm, para que la maquina haga varior cortes y de esa manera no se fuerza mucho.

**Paso 7**: Creamos un 2d pocket para rebajar el grosor de las patas. Seleccionando las 4 caras y nuevamente aplicamos el Paso 6 de multiple depths.

**Paso 8**: Repetimos el paso 6 seleccionando los bordes inferiores de cada una de las piezas y en la sección "Geometry" debemos seleccionar la casilla de tabs y cambiar los siguientes valores. Tab Height=3, Tab distance= 350. Para que al cortar la plancha las piezas no se desprendan y provoque una falla con la fresa.

----- 
### 4) Videos

##### Parte 1
{{< video-local src="4.m4v" >}}

---- 

##### Parte 2
{{< video-local src="5.m4v" >}}
 
 ---


### 5) Galeria 
 {{< gallery dir="/img/galeria2/" />}} {{< load-photoswipe >}}

---
[[Volver Arriba]]() 