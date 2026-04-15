# apuntes-unidad-2
apuntes de la unidad 2 graficacion 


# 📑 Menú de contenidos

- [2.1. Transformación bidimensional](#21-transformacion-bidimensional)
  - [2.1.1. Traslación](#211-traslacion)
  - [2.1.2. Escalamiento](#212-Escalamiento)
  - [2.1.3. Rotación](#213-Rotacion)
  - [2.1.4. Sesgado](#214-sesgado)
- [2.2. Representación matricial de las transformaciones bidimensionales](#22-representacion-matricial-de-las-transformaciones-bidimensionales)
- [2.3. Trazo de líneas curvas](#23-trazo-de-lineas-curvas)
  - [2.3.1. Bezier](#231-Bezier)
  - [2.3.2. B-spline](#232-b-spline)
- [2.4. Fractales](#24-fractales)
- [2.5. Uso y creación de fuentes de texto](#25-uso-y-creacion-de-fuentes-de-texto)



## 2.1. transformación bidimensional

La transformación bidimensional es el conjunto de técnicas que permiten cambiar la posición, el tamaño o la orientación de una figura en un plano. Se usan para mover objetos, hacerlos más grandes o más pequeños, girarlos o darles una forma inclinada. Estas operaciones son muy importantes en la graficación porque nos ayudan a representar y manipular dibujos y datos de manera visual.

**Tipos de transformaciones:**
- **Traslación:** consiste en mover una figura de un lugar a otro sin modificar su forma ni su tamaño. Por ejemplo, desplazar un cuadrado hacia la derecha.
- **Escalamiento:** sirve para aumentar o reducir el tamaño de una figura. Por ejemplo, hacer un círculo el doble de grande.
- **Rotación:** permite girar una figura alrededor de un punto fijo. Por ejemplo, girar una línea 90 grados.
- **Sesgado:** cambia la forma de una figura inclinándola hacia un lado, como convertir un rectángulo en un paralelogramo.

**Importancia:**
Las transformaciones bidimensionales son la base de muchas aplicaciones gráficas. Gracias a ellas se pueden crear animaciones, modificar dibujos y representar información de manera clara y atractiva. Son útiles en matemáticas, diseño gráfico, ingeniería y programación.

**Ejemplo sencillo:**
Imagina un triángulo en el plano. Si lo trasladas, se moverá a otra posición. Si lo escalas, se hará más grande o más pequeño. Si lo rotas, cambiará su orientación. Con estas operaciones simples se pueden construir escenas más complejas y dinámicas.
### 2.1.1. Traslación

La traslación es una transformación bidimensional que consiste en mover una figura de un lugar a otro dentro del plano. Lo importante es que la figura no cambia su forma, su tamaño ni su orientación, simplemente se desplaza a una nueva posición. Cada punto de la figura se mueve la misma cantidad en la dirección que se indique.

Por ejemplo, si tenemos un cuadrado en cierta posición y aplicamos una traslación hacia la derecha, todo el cuadrado se moverá en esa dirección, manteniendo su aspecto original. De la misma manera, si lo trasladamos hacia arriba, la figura se moverá hacia esa zona del plano.

**Características principales de la traslación:**
- No altera la forma de la figura.
- No modifica el tamaño.
- No cambia la orientación.
- Solo cambia la ubicación.

**Ejemplo sencillo:**
Imagina un triángulo dibujado en el plano. Si lo trasladamos 3 unidades hacia la derecha y 2 hacia arriba, el triángulo aparecerá en una nueva posición, pero seguirá siendo exactamente igual al original.

**Importancia:**
La traslación es muy útil en graficación porque permite colocar objetos en diferentes posiciones dentro de una escena. Gracias a ella se pueden organizar figuras, mover elementos en una animación y construir representaciones más completas sin necesidad de redibujar cada objeto.
### 2.1.2. Escalamiento

El escalamiento es una transformación bidimensional que se utiliza para cambiar el tamaño de una figura en el plano. Con esta operación podemos hacer que un objeto se vea más grande o más pequeño, pero manteniendo su forma original. Es como acercar o alejar una imagen sin modificar sus proporciones.

Cuando aplicamos un escalamiento, cada punto de la figura se multiplica por un valor que indica cuánto debe crecer o reducirse. Si el valor es mayor que uno, la figura se amplía. Si el valor está entre cero y uno, la figura se reduce. Lo importante es que la figura conserva su orientación y su forma, solo cambia su tamaño.

**Características principales del escalamiento:**
- Permite aumentar o disminuir el tamaño de una figura.
- Mantiene la forma original, aunque puede cambiar las proporciones si se escala diferente en cada dirección.
- No altera la orientación de la figura.
- Se aplica a todos los puntos de la figura de manera uniforme.

**Ejemplo sencillo:**
Imagina un cuadrado dibujado en el plano. Si aplicamos un escalamiento con un valor de 2, el cuadrado se hará el doble de grande. Si aplicamos un valor de 0.5, el cuadrado se reducirá a la mitad de su tamaño original. En ambos casos, seguirá siendo un cuadrado, solo que más grande o más pequeño.

**Importancia:**
El escalamiento es muy útil en graficación porque permite ajustar el tamaño de los objetos dentro de una escena. Gracias a esta transformación se pueden crear efectos de zoom, representar figuras en diferentes escalas y construir animaciones en las que los objetos crecen o disminuyen de manera dinámica.
### 2.1.3. Rotación

La rotación es una transformación que se utiliza para girar una figura alrededor de un punto fijo dentro del plano. Ese punto puede ser el origen de coordenadas o cualquier otro que se elija como centro de giro. Al aplicar una rotación, la figura conserva su forma y su tamaño, pero cambia la dirección en la que está orientada. Es como tomar una hoja con un dibujo y girarla sin modificar el dibujo en sí.

Cuando hablamos de rotación, lo más importante es el ángulo de giro. Este ángulo indica cuánto se va a girar la figura y en qué sentido. Puede ser en sentido horario (como las manecillas del reloj) o en sentido antihorario. Por ejemplo, una rotación de 90 grados en sentido antihorario hará que una figura que estaba apuntando hacia la derecha ahora apunte hacia arriba.

**Características principales de la rotación:**
- Mantiene el tamaño y la forma de la figura.
- Cambia únicamente la orientación.
- Se realiza alrededor de un punto fijo.
- El ángulo de giro determina la nueva posición.

**Ejemplo sencillo:**
Imagina un rectángulo colocado en posición horizontal. Si lo rotamos 90 grados alrededor del origen, el rectángulo quedará en posición vertical. Si lo rotamos 180 grados, quedará invertido, apuntando hacia el lado contrario. En todos los casos sigue siendo el mismo rectángulo, solo que orientado de manera distinta.

**Aplicaciones prácticas:**
La rotación es muy útil en graficación porque permite mostrar objetos desde diferentes ángulos. Se utiliza en animaciones para simular movimiento, en diseño gráfico para dar dinamismo a las figuras y en ingeniería para representar piezas que deben observarse desde distintas perspectivas. También es común en videojuegos, donde los personajes y objetos giran para interactuar con el entorno.

**Ejemplo cotidiano:**
Un ventilador es un buen ejemplo de rotación. Sus aspas giran alrededor de un eje central, manteniendo siempre la misma forma y tamaño, pero cambiando continuamente de orientación. Este mismo principio se aplica en graficación para dar la sensación de movimiento.
### 2.1.4. sesgado

El sesgado es una transformación que se utiliza para inclinar una figura en el plano, como si la empujáramos hacia un lado sin mover toda la base. A diferencia de otras transformaciones, aquí la figura se deforma: lo que antes era un rectángulo perfectamente vertical puede convertirse en un paralelogramo inclinado. Es una manera de alterar la forma sin modificar el tamaño total.

Cuando se aplica en el eje horizontal, la parte superior de la figura se desplaza hacia la derecha o hacia la izquierda, mientras la parte inferior permanece fija. Si se aplica en el eje vertical, la figura se inclina hacia arriba o hacia abajo. El resultado es una figura que parece estar “torcida” o “inclinada”, pero que conserva sus proporciones generales.

El sesgado tiene un papel importante en graficación porque permite simular efectos visuales que dan más realismo. Por ejemplo, se puede usar para representar la sombra de un objeto, para dar la sensación de que una figura está vista en perspectiva, o para crear animaciones en las que los objetos se deforman al moverse. Es una herramienta que aporta dinamismo y variedad a las escenas.

Un caso cotidiano que ayuda a entenderlo es el de una torre de bloques que se inclina porque alguien empujó la parte superior. La base sigue en el mismo lugar, pero toda la torre se ve inclinada. Esa misma idea es la que se aplica en el sesgado dentro de un plano de graficación.
## 2.2. representación matricial de las transformaciones bidimensionales

Las transformaciones bidimensionales no solo se describen con palabras, también se pueden expresar mediante matrices. Una matriz es una forma ordenada de números que permite aplicar operaciones matemáticas de manera más rápida y organizada. En graficación, las matrices son muy útiles porque permiten calcular de forma automática cómo cambia cada punto de una figura cuando se aplica una transformación.

La idea principal es que cada punto de una figura se puede representar con sus coordenadas en el plano (x, y). Cuando queremos trasladar, escalar, rotar o sesgar la figura, usamos una matriz que contiene los valores necesarios para realizar esa operación. Al multiplicar la matriz por las coordenadas del punto, obtenemos la nueva posición del punto transformado. De esta manera, toda la figura se transforma de forma ordenada y precisa.

**Ventajas de usar matrices en las transformaciones:**
- Permiten aplicar cálculos de manera rápida y sistemática.
- Facilitan la programación de gráficos en computadoras.
- Hacen posible combinar varias transformaciones en una sola operación.
- Reducen errores, ya que el proceso es matemático y exacto.

**Ejemplo:**
Imagina que tienes un dibujo formado por muchos puntos. Si quisieras moverlo a mano, tendrías que calcular uno por uno dónde queda cada punto después de la transformación. Con las matrices, basta con aplicar la operación a todos los puntos de forma automática, como si fuera una receta que se repite igual para cada uno. Esto ahorra tiempo y asegura que la figura se transforme correctamente.

**Aplicaciones:**
La representación matricial se usa en animaciones, videojuegos, diseño gráfico y simulaciones. Gracias a ella, los programas pueden mover personajes, cambiar el tamaño de objetos, girar imágenes o darles perspectiva sin necesidad de redibujar todo desde cero. Es una herramienta fundamental para que la graficación sea eficiente y precisa.
import bpy

class ModalMoveOperator(bpy.types.Operator):
    """Controlar objeto con flechas izquierda/derecha/arriba/abajo"""
    bl_idname = "object.modal_move_operator"
    bl_label = "Modal Move Operator"

    def modal(self, context, event):
        # 1. Referencia al objeto por nombre
        obj = bpy.data.objects.get("Stroke")

        # 2. Detectar eventos de teclado (Flechas)
        if event.type == 'LEFT_ARROW' and event.value == 'PRESS':
            # Traslación en X negativo
            obj.location.x -= 0.5

        elif event.type == 'RIGHT_ARROW' and event.value == 'PRESS':
            # Traslación en X positivo
            obj.location.x += 0.5

        elif event.type == 'UP_ARROW' and event.value == 'PRESS':
            # Subir en Z
            obj.location.z += 0.5

        elif event.type == 'DOWN_ARROW' and event.value == 'PRESS':
            # Bajar en Z
            obj.location.z -= 0.5

        # 3. Permitir salida del modo controlador
        elif event.type in {'ESC'}:
            print("Control finalizado.")
            return {'FINISHED'}

        return {'RUNNING_MODAL'}

    def invoke(self, context, event):
        context.window_manager.modal_handler_add(self)
        print("Control activo: Usa flechas IZQ/DER/ARRIBA/ABAJO. Presiona ESC para salir.")
        return {'RUNNING_MODAL'}
lo que hace el codigo es 
# Registro del operador en Blender
bpy.utils.register_class(ModalMoveOperator)

# Ejecutar el operador automáticamente al correr el script
bpy.ops.object.modal_move_operator('INVOKE_DEFAULT')
Definición del operador  
Se crea una clase llamada ModalMoveOperator. Esta clase define cómo se comporta el operador dentro de Blender. El operador se registra con un nombre único (object.modal_move_operator) y un título visible (“Modal Move Operator”).

Referencia al objeto  
Dentro del método modal, el script busca un objeto llamado "Stroke" en la escena. Ese será el objeto que se moverá.

Detección de teclas  
El operador está atento a las teclas de flechas:

Flecha izquierda: mueve el objeto hacia la izquierda (disminuye su posición en X).

Flecha derecha: mueve el objeto hacia la derecha (aumenta su posición en X).

Flecha arriba: sube el objeto (aumenta su posición en Z).

Flecha abajo: baja el objeto (disminuye su posición en Z).

Salir del modo control  
Si presionas la tecla ESC, el operador se detiene y muestra un mensaje de que el control terminó.

Activación del operador  
El método invoke inicia el operador y muestra un mensaje en la consola:
“Control activo: Usa flechas IZQ/DER/ARRIBA/ABAJO. Presiona ESC para salir.”

Registro y ejecución  
Al final, el script registra el operador en Blender y lo ejecuta automáticamente. Así, al correr el script, ya puedes controlar el objeto "Stroke" con las flechas
## 2.3. trazo de líneas curvas

El trazo de líneas curvas es una técnica fundamental en graficación porque permite representar formas más naturales y suaves que las líneas rectas. Mientras las rectas se usan para figuras geométricas simples, las curvas son necesarias para dibujar círculos, arcos, ondas y cualquier forma orgánica que aparezca en la vida real. Gracias a las curvas, los gráficos adquieren mayor realismo y expresividad.

Para construir una curva en el plano se utilizan puntos de referencia que marcan su trayectoria. Estos puntos pueden ser extremos, intermedios o de control, y determinan cómo se va a doblar la línea. En graficación por computadora, existen distintos métodos para generar curvas, como las curvas polinómicas, las curvas de Bézier o las curvas spline. Cada una tiene sus propias reglas, pero todas buscan el mismo objetivo: crear una línea continua y suave que pase por ciertos puntos o se acerque a ellos.

**Características del trazo de curvas:**
- Permite representar formas suaves y naturales.
- Se define a partir de puntos de referencia o control.
- Puede ser abierta (como una onda) o cerrada (como un círculo).
- Es más flexible que las líneas rectas, ya que se adapta a diferentes trayectorias.

**Aplicaciones prácticas:**
El trazo de curvas se utiliza en diseño gráfico, animación, arquitectura y modelado 3D. Por ejemplo, para dibujar el contorno de un personaje, para diseñar una carretera en un plano, o para representar la trayectoria de un objeto en movimiento. Las curvas también son esenciales en tipografía, ya que las letras se forman con combinaciones de líneas rectas y curvas.

**Ejemplo:**
Piensa en la forma de una ola del mar o en el contorno de una hoja. Ninguna de esas figuras puede representarse solo con rectas; necesitan curvas para mostrar su forma real. En graficación, el trazo de curvas permite reproducir esas formas de manera precisa y atractiva.
### 2.3.1. Bézier

Las curvas de Bézier son un tipo especial de línea curva que se utiliza mucho en graficación y diseño digital. Se caracterizan porque se construyen a partir de puntos de control que determinan la forma de la curva. Estos puntos no siempre están sobre la curva, pero influyen en la dirección y la inclinación que tendrá. Gracias a este método, se pueden crear curvas suaves y precisas con un control sencillo.

El concepto fue desarrollado por el ingeniero Pierre Bézier, quien trabajaba en la industria automotriz y necesitaba una forma matemática para diseñar las superficies de los autos. Desde entonces, las curvas de Bézier se han convertido en una herramienta básica en programas de dibujo, animación y modelado.

**Características principales:**
- Se definen por un conjunto de puntos de control.
- La curva siempre pasa por el primer y el último punto.
- Los puntos intermedios sirven para guiar la forma de la curva.
- Permiten crear líneas suaves y continuas con gran precisión.

**Aplicaciones prácticas:**
Las curvas de Bézier se usan en tipografía para diseñar letras, en programas de dibujo vectorial como Illustrator o Inkscape, en animación para definir trayectorias de movimiento y en modelado 3D para dar forma a superficies. También son comunes en interfaces gráficas, donde se emplean para crear transiciones y efectos visuales.

**Ejemplo:**
Cuando dibujas una línea curva en un programa de diseño y aparecen unos manejadores que puedes mover para ajustar la forma, en realidad estás trabajando con una curva de Bézier. Esos manejadores son los puntos de control que determinan cómo se dobla la curva.
### 2.3.2. B-spline

Las curvas B-spline son un tipo de curva muy utilizada en graficación y modelado porque permiten construir líneas suaves y flexibles a partir de varios puntos de control. A diferencia de las curvas de Bézier, las B-spline no siempre pasan por todos los puntos de control, sino que los usan como guía para definir la trayectoria. Esto hace que las curvas sean más estables y fáciles de manejar cuando se trabaja con figuras complejas.

El nombre “B-spline” proviene de “Basis spline”, que significa que la curva se construye a partir de funciones base que se combinan para dar forma a la línea. Gracias a este método, se pueden crear curvas largas y continuas sin necesidad de recalcular todo desde el inicio, lo que resulta muy eficiente en programas de diseño y animación.

**Características principales:**
- Se definen por varios puntos de control que guían la forma de la curva.
- La curva no necesariamente pasa por todos los puntos, pero se aproxima a ellos.
- Permiten unir varios segmentos de manera continua y suave.
- Son más flexibles que las curvas de Bézier cuando se trabaja con muchas secciones.

**Aplicaciones prácticas:**
Las curvas B-spline se usan en diseño asistido por computadora (CAD), en animación para definir trayectorias complejas, en modelado 3D para crear superficies suaves y en gráficos vectoriales para dibujar formas orgánicas. También son comunes en arquitectura y en ingeniería, donde se necesitan curvas precisas para representar planos y estructuras.

**Ejemplo:**
Imagina el trazado de una carretera que debe pasar cerca de varios pueblos. La curva no tiene que pasar exactamente por cada pueblo, pero sí debe acercarse a ellos siguiendo una trayectoria suave. Ese tipo de trazado se puede representar con una curva B-spline, que se adapta a los puntos de control sin perder continuidad.
![referencia de persona corriendo](./images/corriendo.png)
![Persona corriendo en blender](./images/corre.png)
## 2.5. Uso y creación de fuentes de texto

En graficación, el manejo de fuentes de texto es tan importante como el trazo de líneas y figuras. El texto no solo transmite información, también forma parte del diseño visual y puede influir en la estética de una escena. Por eso, es necesario comprender cómo se utilizan las fuentes y cómo se pueden crear nuevas para adaptarse a diferentes necesidades.

El **uso de fuentes** implica seleccionar un estilo tipográfico adecuado para el contexto. Cada fuente tiene características propias: algunas son más legibles, otras más decorativas, algunas transmiten formalidad y otras dinamismo. En aplicaciones gráficas y programas de diseño, se pueden cargar fuentes ya existentes en el sistema o importar tipografías externas para ampliar las opciones.

La **creación de fuentes** es un proceso más especializado. Consiste en diseñar cada carácter (letras, números y símbolos) siguiendo un estilo coherente. Para ello se utilizan herramientas de dibujo vectorial que permiten definir curvas y líneas con precisión, como las curvas Bézier. Una vez diseñados los caracteres, se agrupan en un archivo de fuente que puede instalarse en el sistema operativo y usarse en cualquier programa.

**Aspectos clave:**
- Las fuentes determinan la apariencia del texto en pantalla o en impresión.
- Se pueden usar fuentes estándar del sistema o importar tipografías externas.
- La creación de fuentes requiere diseñar cada carácter con coherencia visual.
- Las curvas y trazos vectoriales son la base para construir letras.

**Aplicaciones prácticas:**
El uso y creación de fuentes es esencial en diseño gráfico, publicidad, interfaces de usuario y animación. Por ejemplo, un logotipo puede requerir una tipografía única creada especialmente para la marca. En videojuegos y películas animadas, las fuentes ayudan a reforzar la ambientación y el estilo visual. También en documentos técnicos, la elección de una fuente clara y legible facilita la comprensión.

**Ejemplo cotidiano:**
Cuando eliges una tipografía distinta en un procesador de texto, estás aplicando el uso de fuentes. Y cuando una empresa diseña su propia tipografía exclusiva para diferenciarse, está creando una fuente personalizada.











