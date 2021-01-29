# Activitats-UF2_1
_Apuntes hechos por: Aitor Perez_
### OBJETIVOS DE LAS PRUEBAS
Muy concretamente, las pruebas sirven sobre todo para conseguir averiguar si el software no hace lo que tiene que hacer o si el software hace lo que no debe hacer.

![N|Solid](https://i.blogs.es/a19bfc/testing/450_1000.jpg)

Para hacer estas pruebas existen diferentes **frameworks** -> es una estructura base utilizada como punto de partida para elaborar un proyecto con objetivos específicos. (Marco de trabajo).

- Estos están formados por:
    * Un conjunto de las mejores prácticas y suposiciones
    * Herramientas comunes
    * bibliotecas
- Utilizaríamos **frameworks** por:
    * Evitar escribir código repetitivo
    * Utilizar buenas prácticas
    * Permitir hacer cosas avanzadas que un usuario no haría
    * Desarrollar más rápido

Con esto podremos lograr unificar el proceso de desarrollo entre desarrolladores.

### FORMA DE LAS PRUEBAS
Existen dos tipos de pruebas, las **dinámicas** y las **estáticas**,  las dinámicas necesita ejecutar el programa para sacar conclusiones de del comportamiento de la aplicación desarrollada mientras que las estáticas se realizan sin necesidad de ejecutar el programa ya que solo nos fijamos en el código fuente.

### ESTRATEGIAS DE PRUEBA
Continuamos en las pruebas, esta vez para hablar de dos tipos de estrategias utilizadas, conocidas como **caja negra** y **caja blanca**, el color no tiene nada que ver, simplemente para diferenciar la que se utiliza para estudiar el sistema desde fuera para comprobar su funcionalidad (caja negra) y la que se examina su código fuente y su ejecución para comprobar su estructura (caja blanca).

![N|Solid](https://jamj2000.github.io/entornosdesarrollo/3/assets/caja_blanca-caja_negra.png)

En las pruebas de caja negra, nos enfocamos solamente en las entradas y salidas del sistema, sin preocuparnos en tener conocimiento de la estructura interna del programa de software. Para obtener el detalle de cuáles deben ser esas entradas y salidas, nos basamos en los requerimientos de software y especificaciones funcionales.

En las pruebas de caja blanca, nos enfocamos nos centramos en el código fuente y en su ejecución comprobando cada uno de sus diferentes métodos. Este método se usa en la fase de pruebas de unidad, aunque también puede ocurrir en otras fases como en las pruebas de sistema o de integración.

### TIPOS DE PRUEBAS
Como norma general, existen dos tipos de pruebas, **las funcionales y las no funcionales**, las pruebas funcionales evaluan el cumplimiento de los requisitos, dentro de ellas, podríamos considerar dentro del saco de funcionales las pruebas unitarias, las de regresión, las de integración, las de humo, las del sistema, las alfa y beta y las de aceptación (validación por parte del cliente). En cambio, las no funcionales evaluan aspectos adicionales como rendimiento, seguridad, ..., donde podríamos relacionar pruebas no funcionales las pruebas de usabilidad, las de rendimiento, las de stress, las de seguridad, las de compatibilidad, las de portabilidad, etc.

![N|Solid](https://testerhouse.com/wp-content/uploads/2019/03/testerhouse-pruebas-funcionales-1024x680.png)

### MECANISMOS DE PRUEBA
Existen dos tipos de mecanismos de prueba, **los manuales y los automáticos**. Los mecanismos de prueba manuales se realizan mediante pruebas realizadas por personal de la empresa o externo mientras que los mecanismos de prueba automáticos se realizan mediante software que se ejecuta de una forma automática comparando los resultados que se esperaban de la prueba con los resultados que se han obtenido.

![N|Solid](https://s03.s3c.es/imag/_v0/770x420/5/c/2/MTP-cortesia--5.jpg)

### INTEGRACIÓN

En este breve apartado me centraré en explicar sobre la integridad. Existen 4 formas de integración:
- Integracióng Big Bang: son un tipo de prueba de integración en el que los elementos software, elementos hardware o ambos son combinados de forma simultánea en un componente o un sistema global en lugar de hacerlo por fases.
- Integración Descendente: Consiste en integrar los módulos moviéndose de arriba abajo por la jerarquía, comenzando desde el esqueleto del programa principal, hasta ir incorporando los módulos subordinados de forma incremental. Tras la incorporación de cada módulo, habrá que realizar la prueba de integración. El programa principal actuará como coordinador de la prueba.
- Integración Ascendente: Consiste en realizar pruebas para verificar que un gran conjunto de partes de software funcionan juntos. Son las pruebas posteriores a las pruebas unitarias y preceden a las pruebas del sistema. 
- Integración Continua: Es una práctica de desarrollo de software mediante la cual los desarrolladores combinan los cambios en el código en un repositorio central de forma periódica, tras lo cual se ejecutan versiones y pruebas automáticas.

Tambien dan a conocer los 4 servidores de integraión **continua**:
- Jenkins
- Bamboo
- TravisCI
- CircleCI

Y como última parte a destacar sobre la integración, remarcar la **cobertura de código**, para empezar, la cobertura de código es una medida que indica el porcentaje de código que ha sido ejecutado durante las pruebas (es posible realizar la cobertura tanto desde el IDE como desde un servicio web apropiado), siempre, se busca que se aproxime lo más cercano al 100% y si llegase a ser un 100%, entonces se ha ejecutado todo el código fuente durante las pruebas, si llegase a ser menor del 100% entonces existe código fuente que no se ha ejecutado durante las pruebas.

### CALIDAD

Para lograr un control de calidad, principalmente, realizaremos las pruebas suficientes para lograr una medición de la calidad, de un producto.
Primero, vamos a diferenciar entre **QA i QC**, QA es un conjunto de actividades para garantizar la calidad en los procesos mediante los cuales se desarrollan los productos mientras que QC es un conjunto de actividades para garantizar la calidad de los productos. Las actividades se centran en identificar defectos en los productos reales producidos.

![N|Solid](https://prd-wret.s3.us-west-2.amazonaws.com/assets/palladium/production/s3fs-public/styles/landing_page_custom_blocks/public/thumbnails/image/QAQC_3.png)
