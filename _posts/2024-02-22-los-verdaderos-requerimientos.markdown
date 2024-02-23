Los verdaderos requerimientos

https://developsense.com/blog/2023/12/the-real-requirements

* * *

# Los verdaderos Requerimientos

Una de las razones por las que el desarrollo y las pruebas de software son un desastre es porque la gente a menudo nombra las cosas sin cuidado.

A Jerry Weinberg le gustaba señalar que el "punto flotante" era el tipo de matemáticas en las que el punto decimal permanecía en el mismo lugar, mientras que en el "punto fijo", el punto decimal se mueve. La gente habla de "computación sin servidor", cuando en realidad quieren decir "computación que utiliza los servidores de otra persona". "Herramientas de prueba sin código"... bueno, siempre hay código; sólo que es código que tú no escribiste.

He aquí un término que está muy mal considerado: "*requerimientos no funcionales*".

Imagina referirte a casi todo lo que hay en los bosques del mundo como "árboles que no son de Navidad". Imagínate hablar de casi todo lo que podemos comer como "alimentos que no son brócoli".

¿Cómo es posible que los requerimientos que importan a la gente hayan llegado a ser agrupados y, hasta cierto punto, desechados lingüísticamente como "requerimientos no funcionales"? Tengo una teoría.

Una parte del problema se debe a las estructuras sociales en el desarrollo de software. La otra es que a menudo tratamos las diferencias entre *funciones, funcionalidades y requisitos* como si fueran lo mismo, y eso puede ser confuso. Empecemos por intentar desenredar todo esto.

La gente utiliza los programas informáticos para realizar tareas, comunicarse, almacenar datos, aprender, entretenerse, ayudarle a resolver problemas y para conseguir cosas que necesita o desea. Tendemos a llamar a esas cosas *requerimientos*.

Los requerimientos pueden verse a través de la lente de los *criterios de calidad*. En [Rapid Software Testing](https://developsense.com/about-rapid-software-testing), en nuestra lista no exhaustiva de criterios de calidad se incluyen la capacidad, la fiabilidad, la facilidad de uso, el carisma, la seguridad, la escalabilidad, la compatibilidad, el rendimiento y la instalabilidad. También hay criterios de calidad que pueden ser importantes para la empresa y la organización de desarrollo, entre las que se incluyen la soportabilidad, la testabilidad, la mantenibilidad, la portabilidad y la localizabilidad. Para cada una de estas familias de categorías, existen subcategorías; puede [encontrarlas aquí](https://www.satisfice.com/download/heuristic-test-strategy-model).

En todo producto hay *funcionalidades*, aspectos del producto que permiten a los usuarios cumplir con sus requerimientos, o que ayudan a defender a los usuarios de pérdidas, daños o problemas de diversa índole. Los criterios de calidad se aplican en distintos grados a la percepción que las personas tienen de cada funcionalidad.

Las *funciones* son aspectos del software que habilitan las funcionalidades. Cuando algo ocurre o cambia en el producto, se debe a las funciones que hay en algún lugar del código. Mueve tu ratón: algunas funciones procesan y rastrean el movimiento, y otras funciones dibujan el puntero en una nueva posición en la pantalla. Pulsa el botón "Guardar", y una función de la aplicación llama a otra función de la aplicación, que a su vez recoge tus datos y luego llama a otra función suministrada por el sistema operativo para escribir una nueva versión del archivo en el disco.

Sean cuales sean las funcionalidades del producto, necesitamos funciones que las hagan realidad. El trabajo principal del desarrollador consiste en crear las funciones necesarias. Para ello, los desarrolladores crean y mantienen funciones para procesar entradas o eventos. Esas funciones invocan a otras funciones, o son invocadas por otras funciones.

La organización social del desarrollo de software tiende -de forma bastante razonable- a poner a los desarrolladores en el centro de atención. Lo vemos en el propio nombre: *desarrollo* de software, y en la sustitución gradual de "programador" por "desarrollador". Tendemos a hablar de requerimientos *funcionales* cuando intentamos expresar cosas que son importantes para los desarrolladores: la necesidad de funciones, y de que las funciones hagan ciertas cosas de cierta manera.

Las funciones son realmente importantes, porque permiten todo lo que ocurre o cambia en el producto. En consecuencia, es una muy buena idea checar la salida de las funciones conforme construimos el producto. La mayoría de las veces, podemos checar la salida funcional de forma mecánica, algorítmica, con código para ejecutar estas funciones y comparar su salida con algún resultado especificado y presumiblemente deseable.

Suele ser muy, *muy* buena idea que los desarrolladores hagan eso. Los desarrolladores son expertos en escribir código, tanto de producción como para checar el mismo código; tienen nociones de lo que quieren que haga el código de producción; y crear y mantener sus propios chequeos sobre la marcha proporciona una retroalimentación muy rápida. Todo eso está muy bien.

La correctitud funcional es obviamente importante, porque si las funciones no producen la salida correcta, o no hacen los cambios correctos, pueden ocurrir cosas malas, o cosas buenas pueden no ocurrir, de manera que no se cumplan los requerimientos de los usuarios. Pero aquí hay una sutil asimetría: la correctitud funcional *no significa* que se cumplan los requerimientos de los usuarios.

Aunque las funciones tienden a ser el foco principal del trabajo de los desarrolladores, en su mayor parte, las propias funciones son invisibles para las personas que utilizan el producto. A esas personas no les interesan realmente las funciones como tales; lo que les interesa son las funcionalidades, las cosas que aportan las funciones. Los usuarios quieren que el software les ayude a hacer su trabajo, que fomente las interacciones con otras personas, que proteja sus datos y su privacidad, etc. Todas las cosas maravillosas que el software puede hacer por ellos. Cuando se trata de eso, las funciones son sólo un medio para conseguir un fin.

Es decir: nuestros clientes no piensan en términos de requerimientos *funcionales* o *no funcionales*; piensan en términos de *requerimientos*. Dado que nuestro objetivo es proporcionar software y servicios útiles a las personas, creo que nosotros también deberíamos pensar así.

Por eso, las pruebas no pueden limitarse a checar los resultados de las funciones. Debemos investigar el riesgo de que los requerimientos -expresados en términos de funcionalidades y criterios de calidad- no se cumplan o sean insatisfactorios. Para ello, debemos adquirir experiencia con el software, explorar sus rincones ocultos y experimentar con él para encontrar problemas. Y debemos hacerlo con un grado de profundidad [justificado por el riesgo](https://developsense.com/blog/2022/01/testing-deep-and-shallow).

Eso no sólo significa hacer pruebas como *usuarios*; significa hacer pruebas como *testers*. Incluye ayudar al equipo a detectar los criterios de calidad que faltan o que han disminuido de alguna manera, en cada paso del proceso. Incluye realizar *pruebas en perspectiva* durante las reuniones de diseño y perfeccionamiento -ejercitar el producto en nuestras mentes antes de tener el producto disponible- para ayudar a los desarrolladores y diseñadores a cortar los problemas de raíz. Implica utilizar datos amplios, variados, representativos o patológicos en nuestros experimentos para comprobar la fiabilidad. Supone sondear el producto en busca de agujeros de seguridad y aplicar carga y estrés para detectar problemas de rendimiento.

Y, por supuesto, incluir pruebas desde la perspectiva de los usuarios. Para ello hay que sumergirse en el mundo de los usuarios. Requiere [pruebas interactivas y experienciales](https://www.developsense.com/blog/2021/08/alternatives-to-manual-testing-experiential-attended-exploratory/) para descubrir si el producto es difícil de aprender, difícil de usar o tiene problemas de accesibilidad. Es decir, hay que ver lo que se siente al utilizarlo, para descubrir los tipos de problemas chequeos de salida de las funciones pueden fácilmente pasar por alto.

Nótese el sutil rechazo cuando expresamos cosas reales que la gente real quiere del producto en términos de requisitos "no funcionales". No hagamos eso.

Si necesitamos referirnos a dimensiones específicas de la calidad, podemos referirnos a ellas directamente (capacidad). Cuando queramos referirnos a grupos específicos de requerimientos, podemos anteponer un adjetivo ("requerimientos de rendimiento" o "requerimientos de accesibilidad"). Pero cuando hablemos en términos más generales, evitemos la etiqueta "no funcional". Llamémoslos simple, directa y claramente por lo que son: *requerimientos*.

Quieren ver un video corto sobre esto? [Aqui esta](https://youtu.be/fjr2GtUwVLQ):