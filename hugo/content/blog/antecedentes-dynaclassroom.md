+++
title = "Antecedentes teóricos y prácticos de DynaClassroom"
subtitle = "De Seymour Papert a Bret Victor"
date = "2025-02-24"
months = [ "2025-02" ]
authors = [ "rafael-luque" ]
authorPhotos = [ "rafael-luque.jpg" ]
draft = "false"
tags = [ "estado-del-arte", "constructivismo", "TUI", "embodied-spatial-programming" ]
summary = ""
background = "caso-de-uso-libro-extendido.jpg"
backgroundSummary = "caso-de-uso-libro-extendido.jpg"
+++

Las tecnologías digitales en la educación deberían cambiar el modo en que se enseña y, en particular, los ordenadores deberían ser herramientas para amplificar la capacidad de los estudiantes.

Nuestra tesis es que un medio real de alfabetización basado en tecnologías digitales debería transformar profundamente nuestra forma de entender la educación, brindándonos nuevos modos de pensar y comunicar, que aumentaran nuestras capacidades como seres humanos, siguiendo la visión de *Douglas Engelbart* en *Augmenting Human Intellect* [^1].

Sin embargo, los ordenadores suelen usarse como mero soporte multimedia de contenidos y métodos pedagógicos tradicionales.

Como ya señaló el profesor Francisco Martínez Sánchez [^2]:

> En cuanto a los cambios metodológicos que la incorporación de los nuevos medios debían propiciar se suele quedar en lo anecdótico...
> 
> Muy al contrario las TIC sirven para reforzar los modelos didácticos que se dice se quieren transformar. No puede ser de otra forma cuando se abandonó todo lo que daba sentido y justificaba la incorporación de medios en la enseñanza, la Tecnología Educativa en definitiva, habiéndonos quedado sólo con la última tecnología.

Afortunadamente, no somos los únicos en sostener estas tesis, sino que nuestro trabajo se enmarca en una larga lista de antecedentes, tanto teóricos como técnicos, que nos sirvieron de gran inspiración en el diseño de este nuevo medio de expresión y aprendizaje que denominamos *DynaClassroom*.

Este post trata de repasar brevemente los principales proyectos e investigaciones que han influido en nuestro proyecto. Desde las teorías de desarrollo cognitivo de *Jean Piaget*, que posteriormente fueron extendidas por las contribuciones de *Seymour Papert* o *Mitchel Resnick*, a los principios de diseño de *Smalltalk* de *Alan Kay*, los precedentes en la aplicación de la *Realidad Aumentada Espacial* (SAR) y las *Interfaces de Usuario Tangibles* (TUI) o la propuesta del paradigma de *Programación Espacial Corpórea* de *Anna Fusté*.

Conceptualmente DynaClassroom se basa en unas pocas ideas fundamentales:
* Permitir el aprovechamiento de nuestros modelos mentales espaciales para comprender y expresar mejor cualquier idea que se quiera explorar.
* La aplicación de la premisa anterior al pensamiento computacional mediante el paradigma de *Programación Espacial Corpórea*.
* Aprendizaje experiencial y pensamiento computacional aplicado.

### Modelos mentales espaciales

Las diferentes teorías del desarrollo cognitivo espacial ven la evolución de los dominios espaciales en el cerebro como un evento que ocurre más temprano o más tarde en la infancia. Sin embargo, la literatura científica coincide ampliamente en que los modelos espaciales creados en nuestro cerebro desde etapas tempranas pueden ser aprovechados para mejorar otras capacidades humanas directamente vinculadas a esas áreas del cerebro.

Nosotros, los humanos, como entidad física, vivimos y existimos en un mundo que percibimos en cuatro dimensiones. En cada momento en el tiempo existimos en una posición en el espacio tridimensional y nos relacionamos con objetos y otras entidades a nuestro alrededor que existen en otra posición en el espacio. Todo lo que hacemos ocurre en dicho espacio. Incluso nuestros sueños tienen lugar dentro de ubicaciones con impresiones espaciales, aunque sean abstractas e imaginarias. Relacionamos todas nuestras acciones con el espacio desde el momento en que nacemos. Esto nos lleva a construir un conjunto de modelos espaciales en nuestro cerebro que gobiernan nuestra forma de interactuar con las cosas casi de manera inconsciente.

Cuando subimos las escaleras, no nos detenemos a calcular cuánto tenemos que mover la pierna para llegar al siguiente escalón; nuestra pierna se mueve la distancia adecuada porque tenemos un modelo mental en nuestro cerebro que ha evolucionado por necesidad y que ha permeado en nuestro cerebro hasta ser parte de él.

La evolución humana nos demuestra cómo nos hemos beneficiado de estos modelos espaciales básicos para construir interfaces mejoradas. Tomemos un ejemplo tan antiguo que su origen exacto aún se desconoce; el ábaco. El ábaco es una herramienta desarrollada para cálculos matemáticos prácticos.

El ábaco tiene una interfaz física y espacial. Desliza hacia un lado para sumar y hacia el otro para restar. Sumar y restar son dos constructos matemáticos que los humanos encontraron abstractos y difíciles de escalar sin una representación física concreta. La solución para aprender y manejar ágilmente estos difíciles constructos matemáticos terminó siendo una interfaz que hacía uso de los modelos espaciales disponibles en nuestro cerebro. La solución fue encontrar una manera de usar nuestra noción espacial de la posición de un objeto para representar y operar con la abstracción matemática.

{{<figure class="img-right" src="/img/blog/abaco.jpg" title="Un ábaco moderno.">}}

Hemos utilizado estas técnicas durante años y hoy en día dependemos aún más de ellas. Un ejemplo por excelencia de esto es la Interfaz de Usuario Gŕafica o GUI, por sus siglas en inglés. Las Interfaces de Usuario Gŕaficas se introdujeron como una forma de simplificar la pronunciada curva de aprendizaje de las interfaces de línea de órdenes (CLI). En 1945, *Vannevar Bush* publicó un ensayo que tituló *"As We May Think"* [^3], hablando sobre el problema de los sistemas actuales de selección y bases de datos. Destacó el hecho de que la mente humana funciona según la asociación, no de acuerdo con sistemas alfabéticos o numéricos. Este ensayo temprano inspiró la creación de *SketchPad* [^4] en 1963 por *Ivan Sutherland*, uno de los programas de ordenador más influyentes de la historia, que se considera el primer programa informático que permitió la manipulación directa de objetos gráficos, pionero en la interacción persona-ordenador y predecesor de los programas de diseño asistido por ordenador (CAD).

{{<figure class="img-post" src="/img/blog/sketchpad.png" title="Usuario manejando SketchPad utilizando un lápiz de luz.">}}

SketchPad hizo uso de modelos mentales espaciales para diseñar objetos geométricos en una interfaz 2D. Esta visión temprana de una interfaz de computadora inspiró la creación del *oN-Line System* (NLS) a finales de los años 60 por *Douglas Engelbart*, quien entre otras cosas, también introdujo el ratón como un nuevo dispositivo de entrada para controlar estas interfaces 2D. Similar al ábaco, el ratón permite al usuario mover su mano a lo largo de un plano en el espacio para controlar un sistema de información. Es un ejemplo ubícuo de cómo nos hemos beneficiado de nuestros modelos mentales espaciales para controlar un sistemas de información no tangible.

{{<figure class="img-post" src="/img/blog/nls.png" title="Usuario utilizando el sistema NLS con el ratón en una mano y el \"teclado de acordes\" en la otra.">}}

{{<figure class="img-post" src="/img/blog/raton.png" title="NLS en 1968 con un ratón de 3 botones y un \"teclado de acordes\" de 5 teclas.">}}

Posteriormente, *Alan Kay* desarrolló una nueva GUI para la computadora *Xerox Alto* que estaba basada en ventanas, ficheros, directorios, etc. colocados en el espacio y controlados por el ratón, el primer "escritorio" de computadora.

Esta nueva Interfaz Gráfica de Usuario colocaba elementos en diferentes posiciones en el plano 2D y hacía uso del *esqueumorfismo* para hacer que los elementos representados se asemejaran a sus contrapartes del mundo real. Además de utilizar modelos mentales visuales que el usuario ya tenía, se hacía uso de modelos mentales espaciales para manipular eficazmente la información en el sistema.

{{<figure class="img-post" src="/img/blog/xerox-alto.png" title="Ordenador Xerox Alto en el que se originaron las GUIs actuales.">}}

Nuestras interfaces comenzaron siendo tridimensionales; como el ábaco. Usábamos objetos 3D que podíamos manipular en el espacio. Sin embargo, con la era de la computación, nuestras interfaces principales se desplazaron hacia pantallas 2D ancladas en un único punto en el espacio donde estaba la unidad de cómputo principal. Las primeras computadoras no permitían el uso del espacio ya que su movilidad era limitada. Con el tiempo, las pantallas se han generalizado y las interacciones con los sistemas se han reducido a un toque de dedo. Los dispositivos móviles han invadido la escena social, pero todavía estamos anclados a las interacciones planas 2D que no hacen uso del espacio ni de la fisicalidad de nuestro entorno.

Paralelamente, se han desarrollado otros tipos de interacciones que aprovechan las interfaces sensoriales de nuestro cuerpo. El reconocimiento de voz y las interfaces cerebro-computadora son tecnologías que se han convertido en un gran foco de atención en la investigación y comienzan a entrar en el panorama comercial.

Todos estos sistemas de entrada/salida que estamos tan ansiosos por avanzar tecnológicamente, podrían ganar mayor valor recuperando el componente espacial sobre el cual se construyeron nuestras interfaces originales.

Por ejemplo, podemos enseñar a un niño cómo funciona la gravedad mostrándoselo en una pantalla o podemos rastrear una pelota física real según cae y proyectar los valores de velocidad en distintos instántes de la caída.

Las soluciones tecnológicas actuales tienden a restringir nuestras interacciones a un mundo plano 2D donde no tenemos que movernos y no hacemos uso de todas las capacidades sensoriales de nuestro ser físico. Sin embargo, la naturaleza tridimensional es lo que nos hace humanos, lo que nos permite agarrar cosas, lo que nos define en el mundo. Como explicamos previamente, nuestros cerebros evolucionan con modelos espaciales que consideran la dimensionalidad de nuestros cuerpos. Interactuar con sistemas que utilizan superficies planas, interfaces de voz o interfaces cerebrales requiere nuevos modelos mentales que tenemos que infundir en nuestras mentes. Actualmente estamos creando estos modelos sin construir sobre los fundamentos de nuestro intelecto. Esa es la razón por la cual las personas mayores tienen dificultades para entender cómo usar una pantalla táctil. Porque es un modelo de interacción que no coincide con ninguno de sus esquemas mentales.

Se podría argumentar que los niños son capaces de adaptarse más rápido a estas nuevas interfaces ya que sus modelos mentales no han evolucionado y permeado tanto. Sin embargo, al ofrecerles interfaces planas, les confinamos a un marco de interacción que restringe su contacto con su entorno físico. Al hacer esto, no se requieren ni se ponen en juego gran parte de las destrezas que los seres humanos han evolucionado durante miles de años. Por ejemplo, pasan de usar sus manos para agarrar un juguete y manipularlo en el espacio, a ofrecerles una tipo de interacción que se reduce a usar únicamente la punta de los dedos para jugar en una pantalla de unos pocas pulgadas de tamaño. La manipulación hábil de objetos y la asimilación de la conciencia espacial se pierden con estos tipos de interacciones.

{{<figure class="img-post" src="/img/blog/niños-manipulando-objetos.png" title="Niños jugando usando la manipulación de objetos físicos.">}}

{{<figure class="img-post" src="/img/blog/niña-manipulando-tablet.png" title="Niña jugando con una pantalla táctil usando un dedo de una mano.">}}

Los modelos de interacción a los que nos estamos moviendo no hacen uso de los dominios espaciales que nuestra mente domina durante la infancia. Esto no significa que no debamos usar estos modelos de interacción, pero creemos que nos podríamos beneficiar mucho de encontrar una manera de aprovechar estos dominios espaciales e integrarlos en un nuevo medio digital.

## Programación Espacial Corpórea

Nuestra tesis es que utilizando el espacio como estructura subyacente y los modelos mentales espaciales como bloques de construcción, podemos diseñar un nuevo entorno para la alfabetización digital que también actúe como plataforma de autoría. Este nuevo medio digital ofrece un entorno perfecto para aprender conceptos de pensamiento computacional mientras se utiliza el medio para construir de forma colaborativa en el espacio.

Con ese fin, proponemos el uso de la *Programación Espacial Corpórea*, o *Embodied Spatial Programming* en inglés, un paradigma de programación propuesto por *Anna Fusté* [^5], que nos permite crear utilizando la dimensionalidad del entorno. La Programación Espacial Corpórea hace uso del espacio y los objetos físicos alrededor del usuario para diseñar nuevos comportamientos y programas que tienen un efecto directo en el entorno físico de la persona. El usuario puede codificar a través de objetos tangibles y mecanismos; el resultado se mostrará inmediatamente a través de contenido digital superpuesto en el entorno físico del usuario como una respuesta instantánea a sus acciones. La capacidad de la Realidad Aumentada (AR) para unir los mundos físico y virtual la convierte en una tecnología adecuada para aplicar los principios de la Programación Espacial Corpórea al diseño de interacciones en nuevas interfaces y aplicaciones educativas.

Cuando programamos, hacemos uso de conjuntos de herramientas complejas y visualizamos el resultado final en otros dispositivos como pantallas, o mecanismos físicos como robots. Es un ejercicio difícil abstraerse del medio de entrada e intentar programar en líneas de texto que luego se convertirán en acciones. Esta forma tradicional de entender la computación puede considerarse, de alguna manera, como la teoría de Alan Kay de “trabajar con imágenes para crear símbolos” revertida donde, en lugar de pasar de "trabajar con Imágenes" a "símbolos", tenemos que configurar en primer lugar estos símbolos para llegar a las imágenes deseadas. Estas diferentes salidas tienen algunas ventajas y desventajas. Por ejemplo, como ya hemos mencionado, la limitación de la pantalla es que es una interfaz bidimensional, una simulación aplanada de nuestra propia realidad. Sin embargo, es capaz de mostrar una amplia variedad de contenido arraigado en el medio digital.

Por otro lado, cuando programamos mecanismos físicos, como los robots de LEGO Mindstorms, podemos tener en cuenta el entorno físico y codificar para una salida tridimensional, pero las interacciones y posibilidades se reducen a unas pocas órdenes limitados por sus características físicas. Los mecanismos físicos no tienen la flexibilidad que puede tener el contenido digital y la pantalla ofrece una simulación en un entorno bidimensional separado de nuestro entorno.

Al participar en la Programación Espacial Corpórea, hacemos uso de la programación tangible pero el resultado se muestra superpuesto a nuestro entorno físico, mediante realidad aumentada, aprovechando la flexibilidad del contenido digital colocado en el espacio y embebido en el entorno del usuario. La programación implica comprender y hacer uso de un lenguaje abstracto para generar una salida en nuestro mundo físico. Esta salida puede cambiar el comportamiento de un robot, cambiar la representación en una pantalla o configurar nuestro termostato para que se encienda cuando estemos a diez minutos de casa. Cuando codificamos, hacemos uso de este lenguaje generando scripts y archivos de texto que actúan como entrada; se interpretan y compilan para generar una salida, a menudo en un sistema separado, ya sea una pantalla, un robot u otro dispositivo.

Con la Programación Espacial Corpórea, esta entrada y salida se fusionan en el mismo entorno; el proceso de codificación ocurre en el espacio, superpuesto en la salida directa del sistema. Se puede decir que el lenguaje de programación está incrustado en el propio espacio. De este modo, el usuario comprende inmediatamente lo que ese código está generando o modificando. Hacemos uso de los tokens físicos como nuestra entrada y mostramos el medio digital superpuesto en el espacio como la salida.

{{<figure class="img-post" src="/img/blog/embodied-spatial-programming-paradigms.png" title="Diferentes paradigmas de programación vs Programación Espacial Corpórea (por Anna Fusté)">}}

Diferentes lenguajes y herramientas de autoría han hecho uso del espacio en 3D como el medio de salida al programar. La Tortuga Logo [^6] de *Seymour Papert* es un claro ejemplo. El usuario programa en un entorno 2D, una pantalla, y la salida se experimenta en 3D, donde la tortuga dibuja en el espacio.

No obstante, la Programación Espacial Corpórea hace uso del espacio, no solo en la salida, sino también en la entrada. El usuario define los comportamientos en el entorno 3D y experimenta los resultados de manera inmediata y directamente vinculados a sus acciones en el espacio 3D.

La idea es tener un paradigma de programación que se adapte a la naturaleza del usuario en lugar de hacer que el usuario se adapte a un sistema complejo que se representa en un entorno completamente desconectado. Creemos que esto hace que la Programación Espacial Corpórea sea un arquetipo perfecto para enseñar conceptos de pensamiento computacional y principios de codificación.

{{<figure class="img-post" src="/img/blog/niños-tortuga-logo.png" title="Niños manipulando el robot torguta de LOGO.">}}

## Aprendizaje Experiencial y Pensamiento Computacional

El currículo educativo ha evolucionado durante las últimas décadas hacia metodologías de aprendizaje basadas en la práctica y enfoques de aprendizaje experiencial. Diferentes teorías psicológicas han intentado encontrar medios adecuados para mejorar el desarrollo cognitivo de los niños considerando diferentes etapas de madurez y niveles. La tecnología ha jugado un papel clave en esta evolución, dando lugar a un conjunto de buenas prácticas que aprovechan el medio computacional, pero también a un vasto número de metodologías que carecen de algunos de los ingredientes esenciales para el desarrollo cognitivo adecuado de los niños. Vale la pena revisar todas estas teorías y enfoques para diseñar interfaces mejoradas que puedan ayudar a avanzar en el currículo educativo.

### Hacia una teoría constructivista del aprendizaje

Para construir un marco para un entorno de aprendizaje, es necesario comprender completamente todos los factores, contextos y procesos que afectarán a un niño durante el curso de sus ciclos de desarrollo cognitivo. Existe un amplio cuerpo de trabajo que explora los procesos mentales del desarrollo de un niño. Unos se basan en el trabajo de *Jean Piaget*, el padre del constructivismo, otros se centraron en enfoques más prácticos como las teorías constructivistas de *Seymour Papert* o los enfoques de aprendizaje creativo de *Mitchel Resnick*. Vale la pena revisar todas estas teorías para poder diseñar sistemas adecuados fundamentados en la psicología humana desde la base.

#### Teoría del desarrollo cognitivo de Piaget

Jean Piaget [^7] es considerado uno de los principales pioneros del constructivismo en el campo de la psicología. Introdujo su teoría del desarrollo cognitivo basada en la idea de que el proceso de desarrollo se conforma por un ciclo de etapas. Estas etapas se basan en la experiencia y la experimentación con acciones, y se construyen una tras otra en cada ciclo. Afirmaba que los niños tenían un papel activo en el proceso de aprendizaje y que, a través de la experimentación y el juego, construían sobre el conocimiento que ya habían adquirido.

Piaget presentó cuatro etapas diferentes en el desarrollo de un niño:

* Etapa "sensoriomotora": de nacimiento a 2 años.
* Etapa "preoperacional": de 2 a 7 años.
* Etapa "operacional concreta": de 7 a 11 años.
* Etapa "operacional formal": de 12 años en adelante.

En la primera etapa "sensoriomotora", el niño necesita estar en contacto con su entorno físico. Piaget asumía que la mente en un niño se desarrollaba endógenamente hasta que el infante tenía la capacidad cognitiva para asimilar el lenguaje. En la etapa "preoperacional", el niño comienza a aprender a hablar, sin embargo, no es capaz de razonar o aplicar la lógica. Es una etapa que él consideraba relacionada con el juego y la simulación. En la etapa "operacional concreta", los niños pueden pensar lógicamente, pero su razonamiento está limitado a las posibilidades físicas. Finalmente, en una etapa más avanzada, la "operacional formal", el niño puede manejar símbolos y el pensamiento abstracto.

Años después, los investigadores comenzarían a darse cuenta de que estas etapas no deberían tratarse como secuenciales, sino más bien como eventos paralelos y continuos. La adquisición de habilidades sensoriomotoras y los principios del desarrollo cognitivo se presentaban como eventos que deberían estar entrelazados para potenciar los procesos de aprendizaje.

#### El construccionismo de Seymour Papert

Siguiendo las teorías del constructivismo de Jean Piaget, Seymour Papert desarrolló lo que él llamó construccionismo. El construccionismo es una ramificación del constructivismo y se basa en la idea de que los niños aprenden creando modelos mentales en sus cerebros a partir de la experiencia y la acción. El aprendizaje por descubrimiento es clave y se construye sobre el conocimiento previamente adquirido. Papert fue un gran defensor del aprendizaje basado en proyectos. Fue matemático, informático y educador, y uno de los pioneros de la inteligencia artificial. Pasó la mayor parte de su carrera trabajando en teorías de aprendizaje y utilizó las nuevas tecnologías como un campo de juego para los métodos de aprendizaje constructionistas.

Los principios del construccionismo sostienen que el proceso de aprendizaje es más efectivo cuando los estudiantes participan en la creación e interacción con objetos tangibles en el entorno físico. Como el propio Papert definió el concepto [^8]:

> La palabra construccionismo es un nemotécnico para dos aspectos de la teoría de la educación científica que subyace a este proyecto. De las teorías constructivistas de la psicología, tomamos una visión del aprendizaje como una reconstrucción en lugar de como una transmisión de conocimiento. Luego extendemos la idea de materiales manipulativos a la idea de que el aprendizaje es más efectivo cuando forma parte de una actividad que el aprendiz experimenta como la construcción de un producto significativo.

Papert defendía firmemente el uso del computador en el aula. El construccionismo fue inicialmente utilizado para enseñar matemáticas; sin embargo, Seymour Papert comenzó a poner énfasis en lo que él llamó pensamiento computacional como una nueva forma de interactuar con la nueva era de la tecnología. Se han desarrollado varios lenguajes de programación y entornos como plataformas para el aprendizaje construccionista y el pensamiento computacional. El propio Papert desarrolló el lenguaje LOGO, que introdujo el concepto de la tortuga programable a los niños de escuela primaria. Otros lenguajes y plataformas que siguen los principios construccionistas son Smalltalk [^9] y Etoys [^10] de Alan Kay y Scratch [^11] de Resnick.

{{<figure class="img-post" src="/img/blog/tortuga-valiant.png" title="Niños controlando la tortuga Valiant a través del lenguaje de programación LOGO de Seymour Papert.">}}

#### Aprendizaje a través del juego

Mitchel Resnick, profesor del MIT Media Lab, inicia su libro *"Lifelong Kindergarten"* [^12] con el ejemplo de *Chen Jining*, el presidente de la Universidad de Tsinghua, la principal universidad de ingeniería en China. Explica cómo Chen Jining estaba preocupado porque los estudiantes chinos, a pesar de tener altos estándares y buenas calificaciones, no estaban realmente preparados para las necesidades de nuestra sociedad constantemente cambiante y evolutiva. Los estudiantes conocían la teoría, sabían cómo resolver problemas matemáticos, pero no tenían la capacidad de pensar creativamente, de formular sus propias preguntas, plantear sus propias inquietudes y resolverlas. Resnick, influenciado por las teorías constructivistas de Papert, habla de la necesidad de forjar una nueva generación de estudiantes que sean curiosos, que piensen más allá y que puedan formular nuevos desafíos basados en el conocimiento que adquieren. Para preparar a los estudiantes para este futuro en constante cambio, **necesitamos moldear pensadores creativos**.

Resnick dirige su grupo "Lifelong Kindergarten" en el MIT Media Lab, donde trabaja hacia una visión del currículo educativo mucho más abierta a la creatividad y al juego libre. Habla del proceso creativo como una *"Espiral de Aprendizaje Creativo"*, significativamente relacionada con las teorías del desarrollo cognitivo de Piaget y las teorías constructivistas de Papert. En su "Espiral de Aprendizaje Creativo", hay cinco etapas diferentes: "Imaginar", "Crear", "Jugar", "Compartir" y "Reflexionar". Se define como un ciclo infinito que se construye en cada iteración.

{{<figure class="img-post" src="/img/blog/espiral-aprendizaje-creativo.png" title="Proceso de la \"Espiral de Aprendizaje Creativo\" de Resnick.">}}

En el grupo Lifelong Kindergarten, Resnick ha desarrollado un marco para el pensamiento creativo basado en cuatro principios básicos: "proyectos", "pasión", "pares" y "juego". Resnick explica cómo crear "proyectos" es esencial para la Espiral de Aprendizaje Creativo y destaca algunos ejemplos en la comunidad de Scratch, donde los usuarios crean proyectos constantemente que les ayudan a desarrollar sus habilidades y creatividad. Como dijo Piaget: "Los niños aprenden mejor cuando están activamente involucrados en construir algo que tiene un significado personal para ellos", por eso la "pasión" es fundamental para el proceso creativo. "Pares" se refiere a la colaboración y al compartir proyectos con otros. Como afirma Resnick: "La creatividad es un proceso social". Finalmente, el último núcleo es "Juego". La experimentación lúdica es clave para prosperar con éxito en el proceso creativo.

{{<figure class="img-post" src="/img/blog/4-Ps.png" title="Las 4 P's del aprendizaje creativo, según Resnick.">}}



### Referencias

[^1]: Sutherlandʼs, I., Engelbart, D.C., Kay, A.C., & Alto, T. (1962). **Augmenting human intellect: a conceptual framework**.
[^2]: Martínez, F. (2016). **Sentado en el andén**. RIITE. Revista Interuniversitaria de Investigación en Tecnología Educativa, 0, 17-22. Doi: http://dx.doi.org/10.6018/riite/2016/258131
[^3]: Rajaraman, V., & Bush, V. (1945). **As we may think**. Resonance, 5, 94-103.
[^4]: I. E. Sutherland. **SketchPad: A man-machine graphical communication system**. AFIPS Conference Proceedings 23, 1963, 323–328.
[^5]: Anna Fusté. 2018. **Hypercubes: Learning Computational Thinking Through Embodied Spatial Programming in Augmented Reality**. Massachusetts Institute of Technology.
[^6]: Seymour Papert. 1980. **Mindstorms: Children, Computers, And Powerful Ideas**.
[^7]:
[^8]:
[^9]:
[^10]:
[^11]:
[^12]: