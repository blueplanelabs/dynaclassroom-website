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

{{<figure class="img-right" src="/img/blog/abaco.jpg" title="Un ábaco moderno.">}}

El ábaco tiene una interfaz física y espacial. Desliza hacia un lado para sumar y hacia el otro para restar. Sumar y restar son dos constructos matemáticos que los humanos encontraron abstractos y difíciles de escalar sin una representación física concreta. La solución para aprender y manejar ágilmente estos difíciles constructos matemáticos terminó siendo una interfaz que hacía uso de los modelos espaciales disponibles en nuestro cerebro. La solución fue encontrar una manera de usar nuestra noción espacial de la posición de un objeto para representar y operar con la abstracción matemática.

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

### Programación Espacial Corpórea

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

### Pensamiento Computacional

#### Más allá de Papert

Logo[^6] fue el primer lenguaje de programación creado para enseñar conceptos de Pensamiento Computacional. Desde su creación, se han desarrollado numerosas otras plataformas y lenguajes de programación con el mismo objetivo ([^10]). Algunas de estas plataformas se inspiran en el enfoque de aprendizaje constructivista de Papert, como Scratch [^11], un lenguaje de programación gratuito y una comunidad en línea donde los usuarios pueden crear sus propias historias interactivas, juegos y animaciones.

Scratch y muchas otras plataformas hacen uso de la programación visual. Alice [^13], AgentSheets [^14], MIT App Inventor [^15], CS Unplugged [^16] o LEGO Mindstorms [^17] son sólo algunas de las plataformas enfocadas en enseñar programación a niños usando conceptos de pensamiento computacional.

{{<figure class="img-post" src="/img/blog/plataformas-educativas.png" title="Algunas plataformas educativas de pensamiento computacional.">}}

Igualmente, durante las últimas décadas, varios estudios de investigación y expertos han afirmado que el pensamiento computacional es esencial para el desarrollo de los niños. Desde que Papert introdujo el término, la comunidad investigadora ha estado impulsando la inclusión del pensamiento computacional en el currículo educativo. Sin embargo, aunque se ha trabajado mucho en muchos contextos educativos diferentes alrededor del mundo, el trabajo relacionado con el pensamiento computacional incorporado en el aula todavía está en sus inicios.

La razón principal radica en que necesitamos que los niños interactúen y jueguen con su entorno. Y tenerlos frente a una pantalla escribiendo líneas de código no es lo ideal para su propio desarrollo. La gran mayoría de estas herramientas educativas se desarrollan en entornos 2D donde el niño interactúa solo con una pantalla y no aprovecha el espacio a su alrededor. Otros, como LEGO Mindstorms, se basan en robótica y mecanismos y la programación se ve limitada por las capacidades físicas inherentes a los mismos.

Existen muchos caminos abiertos y oportunidades para explorar y también mucho espacio para mejorar en el ámbito educativo. El Pensamiento Computacional conforma un marco que no solo es bueno para aprender sobre el medio informático, sino que pensamos que también debería convertirse en una infraestructura sólida para el aprendizaje en otras muchas áreas del conocimiento como Matemáticas, Física, Historia, Literatura, Música, etc.

#### Aprendizaje empleando pensamiento computacional

El Pensamiento Computacional es mucho más que saber cómo programar. El pensamiento computacional es una forma de entender e interactuar con el mundo. Pensar computacionalmente no significa "pensar como una máquina", de la misma manera que aprender sobre programación no significa solo aprender a codificar. Como dice *Bret Victor* [^18]:

>Una persona no es una máquina, y no debería ser obligada a pensar como una.

Aprender sobre programación significa ser capaz de entender ciertas construcciones de código que potenciarán nuestra forma de abordar un problema y encontrar una solución. Como ya hemos mencionado, Papert puso mucho esfuerzo en desarrollar Logo, un lenguaje de programación destinado a fines educativos y enfocado en aprender sobre programación. Varios otros pioneros en el campo han presentado otras plataformas y lenguajes, así como investigaciones relevantes sobre el tema de aprender sobre programación.

Uno de los ejemplos más notables fue desarrollado por *Alan Kay*, un científico de la computación que ha dedicado gran parte de su vida al desarrollo de tecnología educativa. Kay diseñó el concepto de *Dynabook*, en 1968 (llamado *The KiddiComp* en ese entonces), como "una computadora personal para niños de todas las edades" [^19]. El concepto de Dynabook fue concebido mucho antes de que se lanzara la primera tableta al mercado. También desarrolló varios lenguajes de programación y plataformas educativas como Etoys [^10]. Etoys es un entorno de autoría y sistema de programación visual para niños construido en Squeak, una implementación de código abierto de Smalltalk. Etoys sirvió como inspiración para el desarrollo de Scratch más adelante. Kay no concibió Squeak y Etoys como herramientas para aprender a codificar. Los diseñó como plataformas con un propósito mayor; plataformas para aprender sobre programación como un paraguas para la asimilación de muchas otras áreas temáticas como la física o las matemáticas.

Es evidente que el estudiante no solo aprende sobre programación, sino que explora y experimenta con una amplia gama de conceptos y competencias transversales como la física, las matemáticas, la escritura o la documentación. Kay ha realizado un trabajo sustancial en el área de la programación visual e interactiva. Creó Smalltalk [^9] como un lenguaje de programación educativo que era orientado a objetos, de tipado dinámico y reflexivo.

{{<figure class="img-post" src="/img/blog/niños-smalltalk.png" title="Un grupo de niños usando Smalltalk en una computadora Xerox Alto en los años 80.">}}

### Espacio y Tangibilidad

#### Programación Visual

La comunidad investigadora ha puesto énfasis en la importancia del espacio y la corporeidad utilizados en metodologías educativas para campos STEM. El cuerpo y la relación con el entorno no solo son esenciales para el desarrollo de habilidades motrices, sino que también pueden beneficiar enormemente la comprensión de conceptos más abstractos como las matemáticas o la física. Nosotros, los humanos, existimos en un mundo tridimensional y nuestro cerebro toma este entorno 3D como referencia. Esta referencia ha servido en el pasado y se ha considerado como un poderoso conducto para enseñar conceptos de ciencia y tecnología a los niños. La utilización de principios espaciales para hacer una interfaz más usable e intuitiva (e instintiva) no es algo nuevo en los sistemas tecnológicos. Esta idea se ha aplicado a interfaces de computadora desde el inicio de la era de la computación. La información y conciencia espacial se ha utilizado como herramienta para diseñar interfaces mejor adaptadas a nuestra naturaleza humana.

Uno de los ejemplos claros de esto es la programación visual. La programación visual es un paradigma de programación poderoso y prevalente que ha estado evolucionando desde los años 60. Utiliza referencias visuales y bloques organizados en un espacio 2D para programar una secuencia regular de órdenes. La programación visual es el primer paradigma de programación que aprovechó nuestros esquemas mentales espaciales para diseñar una mejor interfaz para una tarea secuencial. La primera interfaz de programación visual fue creada en 1968. En aquel entonces, *Tom Ellis* creó *GRAIL* [^20], *GRAphical Input Language*, donde los usuarios dibujaban diagramas de flujo para escribir software.

{{<figure class="img-post" src="/img/blog/grail.png" title="Tom Ellis usando una tableta para interactuar con GRAIL en los años 60.">}}

Desde entonces, se han desarrollado muchas otras plataformas y entornos de programación, especialmente para aprender sobre programación utilizando principios espaciales. Un ejemplo de esto es AgentSheets [^14], un sistema de programación visual orientado a dominios; VVVV [^21], una plataforma de programación basada en nodos para programar gráficos; o el Reality Editor [^22], una herramienta para programar objetos inteligentes en Realidad Aumentada.

#### Trabajar con Imágenes crea Símbolos

Alan Kay trabajó en la aplicación de los principios de la programación visual en entornos de aprendizaje para niños. Inspirado por las teorías de Seymour Papert y Jean Piaget, Kay intentó comprender cómo la noción espacial era esencial al abstraer de la realidad y al intentar pensar en el medio computacional.

Si miramos atrás a las teorías del desarrollo cognitivo de Piaget, éste explicó cómo existen diferentes etapas en el desarrollo de un niño. Una primera etapa sensoriomotora donde el niño necesita estar en contacto con su entorno físico; una etapa más avanzada donde el niño puede reconocer patrones; y las etapas finales donde el niño puede manejar símbolos y pensar de manera abstracta. Años después, los investigadores comenzaron a darse cuenta de que estas etapas no deberían tratarse como secuenciales, sino más bien como eventos paralelos y continuos.

Para hacer un símil con las teorías de Piaget, Alan Kay habló sobre la idea de que *"Trabajar con Imágenes crea Símbolos"* [^23]. Como se mencionó anteriormente, Kay es un científico de la computación y es bien conocido por su trabajo en lenguajes de programación visual. Intentó explicar cómo el proceso de aprendizaje se volvería mucho más rico si combináramos todas las etapas de aprendizaje de Piaget. Si los niños pudieran hacer uso del espacio y la fisicalidad de su entorno mientras reconocen patrones y entienden símbolos, el proceso de aprendizaje sería mucho más rico y rápido.

{{<figure class="img-post" src="/img/blog/doing-with-images-makes-symbols.png" title="\"Trabajar con Imágenes Crea Símbolos\" de Alan Kay (imagen de Anna Fusté).">}}

#### Interfaces de Usuario Tangibles

En paralelo a todas las teorías relacionadas con el razonamiento espacial y el desarrollo cognitivo, ha habido muchas investigaciones intentando crear experiencias de aprendizaje que potencien cada una de las etapas de desarrollo piagetianas por separado. Sin embargo, no se ha hecho mucho esfuerzo en intentar combinarlas todas para el aprendizaje. Los enfoques actuales para enseñar pensamiento computacional y programación están basados en pantallas. No obstante, somos criaturas físicas. Como menciona Bret Victor [^24]:

>Vivimos en un mundo tridimensional. Nuestras manos están diseñadas para mover y rotar objetos en tres dimensiones, para recoger objetos y colocarlos sobre, bajo, al lado y dentro de otros. Ninguna criatura en la tierra tiene una destreza que se compare con la nuestra.

Piaget también abogaba por introducir interacciones físicas al diseñar métodos educativos. Destacó la importancia de las acciones físicas hacia los objetos para abstraer de la realidad:

>...hay acciones individuales como lanzar, empujar, tocar, frotar. Son estas acciones individuales las que la mayoría de las veces dan lugar a la abstracción de los objetos.

{{<figure class="img-right" src="/img/blog/metadesk.png" title="Sistema metaDESK.">}}

Siguiendo estos mismos principios, se crearon las Interfaces de Usuario Agarrables. Hoy en día se les llama *Interfaces de Usuario Tangibles* (TUIs) y se basan en la manipulación de tokens físicos en el espacio para controlar una interfaz digital. En 1997 en el MIT Media Lab, *Hiroshi Ishii* y *Brygg Ullmer* [^25] publicaron un artículo donde hablaban sobre la conexión entre bits y átomos. Este artículo se centró en la unión entre el ciberespacio y el entorno físico. Ishii y Ullmer señalaron que habíamos pasado de usar objetos físicos para medir eventos en el mundo, a usar solo computadoras y pantallas como herramientas únicas de medición. En este artículo, Ishii y Ullmer intentaron expresar su voluntad de unificar la riqueza del mundo físico con la interacción humano-computadora. Las Interfaces de Usuario Tangibles son una respuesta a esta necesidad. Uno de los ejemplos que presentaron en su investigación es *metaDESK*. El sistema metaDESK es una plataforma desarrollada en el grupo de Medios Tangibles en el MIT Media Lab para explorar las TUIs. La plataforma permite el uso de gráficos 2D y 3D en una pantalla, y la manipulación de varios objetos físicos detectados por una matriz de sensores ópticos, mecánicos y electromagnéticos.

La investigación de Ishii y Ullmer desencadenó el desarrollo de una serie de nuevos proyectos y más investigaciones relacionadas con esta área. Uno de los proyectos más exitosos que utilizan las TUIs hasta el momento es *reacTable* [^26], una plataforma de edición musical. 

Varios estudios de investigación han afirmado cómo las Interfaces de Usuario Tangibles son beneficiosas para la usabilidad y la interacción natural de un sistema [^27]. No solo mejoran los métodos de interacción humano-computadora, sino que también aumentan los resultados de aprendizaje si se utilizan en un entorno educativo [^28].

#### Programación Tangible

De manera similar a cómo las Interfaces de Usuario Tangibles (TUIs) pueden aumentar el rendimiento en entornos de aprendizaje, existe evidencia de cómo la programación tangible puede ayudar a los usuarios a comprender mejor sus sistemas de programación [^29].

{{<figure class="img-right" src="/img/blog/algoblock.png" title="Grupo de niños usando el sistema AlgoBlock.">}}

La gran mayoría de plataformas que enseñan pensamiento computacional están basadas en pantallas en línea, donde el estudiante se desconecta de su propia realidad física y se aísla de los demás, permaneciendo inmóvil mirando su propio dispositivo. Es por esto que, en paralelo a todo este movimiento de sistemas basados en pantallas en línea, los investigadores han estado reconociendo la importancia de la corporeidad y la manipulación física en las experiencias de aprendizaje. La programación tangible se inspira en estas teorías cognitivas y se han desarrollado diferentes herramientas siguiendo estas líneas de pensamiento. *AlgoBlock* [^30], *Tangible Programming Bricks* [^29] o *CyberPLAYce* [^32], entre muchos otros, son algunos de los innumerables ejemplos de plataformas de programación que utilizan bits físicos para enseñar sobre programación. Si tomamos AlgoBlock como ejemplo, el sistema permite a los estudiantes planificar y construir procedimientos en grupo usando bloques físicos. El niño no programa líneas de código en una pantalla, sino que, en cambio, utiliza bits físicos para diseñar sus programas y secuencias. Luego pueden observar el resultado de sus acciones en una pantalla.

Un enfoque similar es utilizado por sistemas como *Tern* [^33] o *Quetzal* [^34], lenguajes de programación más recientes que hacen uso de los mismos principios. Ambos fueron desarrollados en la Universidad de Tufts por *Michael S. Horn* y se centran en la idea de hacer que las interfaces de programación sean más accesibles para el aula, utilizando materiales simples como el papel para crear entradas de programación en el espacio.

{{<figure class="img-post" src="/img/blog/tern-quetzal.png" title="Sistemas de programación tangible Tern y Quetzal.">}}

Los proyectos mencionados son buenos ejemplos de programación tangible. Las entradas del sistema se disponen en el espacio, aprovechando el entorno físico del usuario. Sin embargo, la salida se visualiza en una pantalla 2D. Esto desvincula las acciones de entrada del usuario de los resultados que el usuario logra. Los bits tangibles que el usuario puede manipular están físicamente desconectados del resultado digital que ocurre en un entorno diferente. Para tener un sistema interactivo y reflexivo que reaccione naturalmente a las acciones del usuario, el contenido digital debería estar vinculado a las fichas físicas y reaccionar a estas de manera instantánea, de modo que el usuario comprenda su funcionalidad automáticamente. Aprender pensamiento computacional con un sistema de programación tangible puede beneficiarse enormemente de la superposición de contenido digital en el espacio.

#### Realidad Aumentada

Con la llegada de la Realidad Virtual (VR) y Realidad Aumentada (AR) y los últimos avances en procesamiento de imágenes y seguimiento espacial, estas nuevas tecnologías establecen un territorio ideal para la experimentación educativa. La AR, en particular, nos permite poner en práctica muchos de los conceptos relacionados con la cognición espacial y el desarrollo cognitivo en el currículo educativo.

Las posibilidades que ofrece la AR nos permiten aprovechar el espacio y fusionar los mundos virtual y físico de una manera que puede beneficiar enormemente las actividades educativas y creativas. Algunos investigadores ya han explorado el uso de la AR como medio para mejorar los enfoques de aprendizaje y creatividad en la educación. Sin embargo, las aplicaciones desarrolladas hasta ahora no aprovechan todo el potencial de esta tecnología. Los nuevos sistemas de seguimiento como ARCore (Google) o ARKit (Apple) y los nuevos dispositivos de visualización montados en la cabeza como Hololens (Microsoft) o Meta 2 (Meta) que han sido lanzados al mercado en los últimos años abren una nueva puerta a la exploración de nuevas metodologías de aprendizaje que involucran el espacio y el entorno físico.

En diferentes intentos de combinar los enfoques digitales basados en pantalla con los tangibles, algunos investigadores han utilizado la AR como un medio flexible que puede potenciar las capacidades de pensamiento espacial en entornos de aprendizaje. *AR Scratch* [^35] es un entorno de autoría para niños para experiencias de realidad aumentada que utiliza el lenguaje de programación Scratch en AR. El sistema permite contenido 2D en una pantalla, haciendo uso de marcadores de imagen frente a la webcam del computador.

Un enfoque similar más enfocado en combinar lo digital con el entorno físico se encuentra en *Color Code* [^36] de *Eric Rosenbaum*. En lugar de marcadores de imagen, Rosenbaum diseñó un conjunto de experimentos que superponen contenido digital dependiendo de códigos de color en el entorno capturado por la webcam.

{{<figure class="img-right" src="/img/blog/dynamicland.png" title="Dynamicland de Bret Victor.">}}

Otro ejemplo del uso de la AR para la educación es *Code Bits* [^37]. Code Bits es un kit de herramientas económico de pensamiento computacional tangible que utiliza patrones planos y AR para enseñar habilidades de programación. El usuario solo necesita papel para crear marcadores de imagen y un smartphone para visualizar el contenido de AR en el espacio. En este caso, los marcadores son planos y necesitan permanecer a la vista para que la aplicación muestre el contenido virtual. El usuario necesita apuntar al tablero en todo momento para que el contenido digital aparezca. La aplicación no tiene conciencia espacial.

Otro sistema que hace uso de AR para el pensamiento computacional en entornos de aprendizaje es *RealTalk* [^38]. RealTalk fue lanzado en 2017 y es *"un entorno para la autoría y uso de medios computacionales con objetos físicos ordinarios - papel, piedras, lo que haya a mano - reconocidos y animados por tecnología instalada en el techo"*. El sistema fue desarrollado por un grupo de investigación liderado por *Bret Victor*. Más tarde, crearon un entorno completo sobre RealTalk, llamado *DynamicLand* [^39], un espacio para la colaboración, programación y experimentación. Bret describió DynamicLand como *"un medio que podemos ver, sentir y manipular"*. DynamicLand es un espacio donde las personas pueden interactuar con objetos y los tokens físicos se fusionan con el contenido digital proyectado desde la tecnología instalada en el techo. El contenido digital 2D se proyecta sobre la superficie de una mesa donde el usuario puede interactuar con él utilizando cualquier tipo de objeto físico. La interacción está limitada a la mesa donde está configurada la tecnología.


### Referencias

[^1]: Sutherlandʼs, I., Engelbart, D.C., Kay, A.C., & Alto, T. (1962). **Augmenting human intellect: a conceptual framework**.
[^2]: Martínez, F. (2016). **Sentado en el andén**. RIITE. Revista Interuniversitaria de Investigación en Tecnología Educativa, 0, 17-22. Doi: http://dx.doi.org/10.6018/riite/2016/258131
[^3]: Rajaraman, V., & Bush, V. (1945). **As we may think**. Resonance, 5, 94-103.
[^4]: I. E. Sutherland. **SketchPad: A man-machine graphical communication system**. AFIPS Conference Proceedings 23, 1963, 323–328.
[^5]: Anna Fusté. 2018. **Hypercubes: Learning Computational Thinking Through Embodied Spatial Programming in Augmented Reality**. Massachusetts Institute of Technology.
[^6]: Seymour Papert. 1980. **Mindstorms: Children, Computers, And Powerful Ideas**.
[^7]: Piaget, Jean. 1971. **The theory of stages in cognitive development**. In D. R. Green, M. P. Ford, & G. B. Flamer, Measurement and Piaget. McGraw-Hill.
[^8]: Papert, Seymour. 1986. **Constructionism: A New Opportunity for Elementary Science Education**. A Proposal to the National Science Foundation, Massachusetts Institute of Technology, Media Laboratory, Epistemology and Learning Group, Cambridge, Massachusetts.
[^9]: Kay, Alan. 1996. **The early history of Smalltalk**. In T. J. Bergin Jr, & R. G. Gibson Jr., History of programming languages---II (pp. 511-598). New York: ACM.
[^10]: Kay, Alan. 2005. **Squeak Etoys, Children & Learning**. Glendale: Viewpoints Research Institute (VPRI).
[^11]: Resnick, M., Maloney, J., Monroy-Hern~ndez, A., Rusk, N., Eastmond, E., Brennan, K., et al. (2009). **Scratch: programming for all**. Communications of the ACM. 52, pp. 60-67. New York: ACM.
[^12]: Resnick, Mitchel. 2017. **Lifelong kindergarten: cultivating creativity through projects, passion, peers, and play**. The MIT Press, Cambridge, Massachusetts.
[^13]: Cooper, S., Dann, W., & Pausch, R. 2000. **Alice: a 3-D tool for introductory programming concepts**. Journal of Computing Sciences in Colleges, 15 (5), 107-116.
[^14]: Repenning, A. 1993. **Agentsheets: a tool for building domain-oriented visual programming environments**. Proceedings of the INTERACT'93 and CHI'93 conference on Human factors in computing systems (pp. 142-143). Amsterdam: ACM.
[^15]: Pokress, S. C., & Dominguez Veiga, J. J. 2013. **MIT App Inventor: Enabling personal mobile computing**. arXiv:1310.2830.
[^16]: Bell, T., Alexander, J., Freeman, I., & Grimley, M. (2009). **Computer science unplugged: School students doing real computing without computers**. The New Zealand Journal of Applied Computing and Information Technology, 13 (1), 20-29.
[^17]: Klassner, F., & Anderson, S. D. (2003). **Lego MindStorms: Not just for K-12 anymore*. IEEE Robotics & Automation Magazine, 10 (2), pp. 12-18.
[^18]: Victor, Bret. 2012. **Learnable programming**. Del sitio web de Bret Victor: http://worrydream.com/#!/LearnableProgramming
[^19]: Kay, Alan. 2011. **A Personal Computer for Children of All Ages**. In Proceedings of the ACM Annual Conference - Volume 1 (ACM ’72).
[^20]: Ellis, T. 0., Heafner, J. F., & Sibley, W. L. (1969). **The GRAIL Project: An experiment in man-machine communications**. Santa Monica: RAND Corporation.
[^21]: VVVV group. 1998. De la web de vvvv: https://vvvv.org/
[^22]: Heun, V., Hobin, J., & Maes, P. (2013). **Reality editor: programming smarter objects**. Adjunct Proceedings of the 2013 ACM conference on Pervasive and ubiquitous computing adjunct publication (pp. 307-310). Zurich, Switzerland: ACM.
[^23]: Kay, Alan. 1987. **Doing with images makes symbols**. De Internet Archive, parte 1: https://archive.org/details/AlanKeyD1987 parte 2: https://archive.org/details/AlanKeyD1987_2
[^24]: Victor, Bret. 2011. **Explorable Explanations**. De la página web de Bret Victor: http://worrydream.com/ExplorableExplanations/
[^25]: Ishii, H., & Ullmer, B. 1997. **Tangible bits: towards seamless interfaces between people, bits and atoms**. Proceedings of the ACM SIGCHI Conference on Human factors in computing systems (pp. 234-241). New York: ACM.
[^26]: Jordá, S., Geiger, G., Alonso, M., & Kaltenbrunner, M. (2007). **The reacTable: exploring the synergy between live music performance and tabletop tangible interfaces**. Proceedings of the 1st international conference on Tangible and embedded interaction (pp. 139-146). New York: ACM.
[^27]: Schneider, B., Jermann, P., Zufferey, G., & Dillenbourg, P. (2011). **Benefits of a Tangible Interface for Collaborative Learning and Interaction**. IEEE Transactions on Learning Technologies, 4 (3), 222 - 232
[^28]: Skulmowski, A., Pradel, S., KOhnert, T., Brunnett, G., & Daniel Rey, G. (2016, January-February). **Embodied learning using a tangible user interface: The effects of haptic perception and selective pointing on a spatial learning task**. Computers & Education, 64-75.
[^29]: McNerney, T. S. (2000). **Tangible programming bricks: An approach to making programming accessible to everyone**. Massachusetts Institute of Technology, Dept. of Architecture. Program In Media Arts and Sciences. Boston: Massachusetts Institute of Technology.
[^30]: Hideyuki, S., & Kato, H. 1993. **AlgoBlock: a Tangible Programming Language - a Tool for Collaborative Learning**. Proceedings of 4th European Logo Conference (pp. 297-303). Athens, Greece.
[^32]: Soleimani, A., Green, K. E., Herro, D., & Walker, I. D. (2016). **A Tangible, Story-Construction Process Employing Spatial, Computational-Thinking**. Proceedings of the The 15th International Conference on Interaction Design and Children (pp. 157-166). Manchester, United Kingdom: ACM.
[^33]: Horn, M. S., & Jacob, R. J. (2007). **Tangible programming in the classroom with tern**. Extended abstracts on Human factors in computing systems (pp. 1965-1970). New York: ACM.
[^34]: Horn, M. S. (2006). **Tangible programming with quetzal: Opportunities for education**. Boston: Tufts University.
[^35]: Radu, I., & MacIntyre, B. (2009). **Augmented-reality scratch: a children's authoring environment for augmented-reality experiences**. Proceedings of the 8th International Conference on Interaction Design and Children (pp. 210-213). Como, Italy: ACM.
[^36]: Rosenbaum, E. (2010). **Color Code**. De la página web: https://www.ericrosenbaum.com/color-code/
[^37]: Goyal, S., Vijay, R. S., Monga, C., & Pratul, K. (2016). **Code Bits: An Inexpensive Tangible Computational Thinking Toolkit For K-12 Curriculum**. Proceedings of the TEI '16: Tenth International Conference on Tangible, Embedded, and Embodied Interaction (pp. 441-447). Eindhoven, Netherlands: ACM.
[^38]: Victor, B., Schachman, T., Te, P., Horowitz, J., & lannini, L. (2016). **Realtalk**. De la web del Human Advancement Research Community: https://harc.ycr.org/project/realtalk/
[^39]: Victor, B. 2017. **DynamicLand**. Página web de DynamicLand: https://dynamicland.org


