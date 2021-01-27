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
