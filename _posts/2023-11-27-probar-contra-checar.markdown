List itemProbar y Checar Refinado

* * *

*Esta es una traducción del post titulado “Testing and Checking Refined” que puedes encontrar en el sitio de Jame Bach*

*https://www.satisfice.com/blog/archives/856*

*Al hacer esta traducción intente utilizar un Español lo mas neutral posible pero no puedo garantizar el resultado, así que antes de mandarme a la Inquisición recomiendo leer el post original o podemos tener una conversación sobre el mismo, checa la pagina de “Contacto” para más información.*

# Probar y Checar Refinado

*Este post ha sido escrito junto con Michael Bolton. Hemos pasado horas discutiendo sobre casi todas las afirmaciones. También agradecemos a Iain McCowatt su rápida revisión y sus comentarios.*

Probar y el uso de herramientas son dos cosas que han caracterizado a la humanidad desde sus inicios. (No son las dos únicas cosas, por supuesto, pero sí dos de las mas importantes). Pero mientras probar es cerebral y en gran medida intangible, el uso de herramientas está a la vista de todos. Las herramientas invaden todos los procesos que tocan y las herramientas cambian esos procesos. De ahí que, durante al menos cien o mil siglos, los más filosóficos de nuestra especie se han preguntado: "¿Esto lo hice yo o lo ha hecho la herramienta? ¿Soy un guerrero o sólo una plataforma de lanzamiento de lanzas? ¿Soy un agricultor o un empujador de arados?". Como dijo Marshall McLuhan "Damos forma a nuestras herramientas, y después nuestras herramientas nos dan forma a nosotros".

Esta evolución puede ser un proceso insidioso que desafía la forma en que nos etiquetamos a nosotros mismos y a las cosas que nos rodean. Podemos ser testigos de cómo la industrialización transforma a los artesanos ebanistas en fábricas de libreros, y eso puede tentarnos a hablar del papel cambiante del ebanista, pero el trabajador de la fábrica de libreros no es, desde luego, un artesano ebanista que ha sufrido una mutación. Los artesanos de la ebanistería siguen ahí -son menos, es cierto-, muy lejos de las fábricas, produciendo gabinetes caros y bien hechos. El experto ebanista (casi estoy motivado como para buscar en Google si existe una palabra especial para experto en ebanistería) sigue siendo solicitado para resolver problemas que IKEA no puede solucionar. Esta situación se da también en los campos de la ciencia y la medicina. Existe en todas partes: ¿cuáles son las implicaciones de la evolución de las herramientas en el trabajo humano especializado? Cualquiera que busque la excelencia en su oficio debe lidiar con el rol de apropiación de las herramientas.

Por lo tanto, no nos sorprenda que probar, hoy en día, sea un proceso que utiliza herramientas de muchas maneras, y esto cuestiona la idea de un probador.

Esto siempre ha sido un problema -llevo trabajando y discutiendo sobre esto desde 1987, y la literatura al respecto se remonta al menos hasta 1961-, pero ha ocurrido algo nuevo: la informática móvil y distribuida a gran escala. Sí, esto es nuevo. En mi opinión, es el mayor reto para probar tal y como lo conocemos desde la aparición de los microordenadores. ¿Por qué exactamente es un reto? Porque además de la complejidad de los productos y plataformas, que no ha dejado de crecer durante las últimas décadas, ahora existe un vasto mercado de productos de software que se espera que sean *distribuidos y actualizados instantáneamente*.

Queremos probar un producto rápidamente. ¿Cómo lo hacemos? Es tentador decir: "¡Hagámoslo con herramientas!". Esto ejerce una enorme presión en los probadores calificados y en quienes diseñan herramientas utilizadas por los probadores. Mientras tanto, las personas que no son expertas en pruebas de software tienen visiones de la industrialización de las pruebas similares a las de las primeras fábricas de libreros. Sí, siempre han existido estas presiones, hasta cierto punto. Ahora, el "desarrollo continuo" ha abierto otro frente en esta guerra.

Creemos que el trabajo cognitivo calificado no es trabajo de fábrica. Por eso es más importante que nunca entender qué es probar y cómo puede apoyarse con el uso de herramientas.

## Probar vs Checar (Testing vs Checking)

Por este motivo, en la metodología de Rapid Software Testing conocemos las diferencias entre los aspectos del proceso de pruebas que pueden hacer las máquinas y los que sólo pueden hacer los humanos calificados. Desde el punto de vista lingüístico, hemos adaptado la palabra inglesa "checking" para referirnos a lo que pueden hacer las herramientas. Esto es muy parecido a la convención establecida desde hace tiempo para distinguir entre "programar" y "compilar". Programar es lo que hacen los programadores humanos. Compilar es lo que hace una herramienta concreta por el programador, aunque lo que hace un compilador pueda parecer, técnicamente, exactamente lo que hacen los programadores. Ahora que lo pienso, nadie habla de programación automatizada ni de programación manual. Hay programación y muchas otras cosas que hacen las herramientas. Una vez que se crea una herramienta que hace lo que un programador, ya no se vuelve a hablar de programación.

Ahora que Michael y yo llevamos más de tres años trabajando con esta distinción, hemos afinado aún más nuestro lenguaje, con definiciones actualizadas y una nueva distinción entre chequeos humanos y chequeos automatizados.

En primer lugar, hablemos de pruebas y chequeos. He aquí las nuevas definiciones propuestas, que pronto sustituirán a las que hemos utilizado durante años (sujetas a revisión y comentario por parte de nuestros colegas):

### Probar

Es el proceso de evaluar un producto aprendiendo sobre él a través de la experiencia, la exploración y la experimentación, lo que incluye en cierta medida: cuestionarlo, estudiarlo, modelarlo, observarlo, hacer inferencias, etc.

Una prueba es una instancia de Probar

### Checar

Es el proceso de hacer evaluaciones aplicando reglas de decisión algorítmicas a observaciones específicas de un producto.

Un chequeo es una instancia de checar

## Notas aclaratorias:

- "evaluar" significa hacer un juicio de valor; ¿es bueno? ¿es malo? ¿aprueba? ¿reprueba? ¿qué tan bueno? ¿qué tan malo? algo así.
- "evaluaciones" como sustantivo se refiere al resultado de la evaluación, que en el contexto de checar es un artefacto de algún tipo; una cadena de bits.
- "aprender" es el proceso de desarrollar la mente propia. Sólo los seres humanos pueden aprender en el sentido más amplio del término, porque nos referimos tanto al conocimiento tácito como al explícito.
- "exploración" implica que probar es intrínsecamente exploratorio. Todas las pruebas son exploratorias hasta cierto punto, pero también pueden estar estructuradas por secuencias de elementos.
- "experimentación" implica la interacción con un objeto y la observación de éste en funcionamiento, pero también nos referimos a "experimentos mentales" que implican una interacción puramente hipotética. Al referirnos a la experimentación, no estamos negando ni rechazando otros tipos de aprendizaje; simplemente intentamos expresar que la experimentación es una práctica que caracteriza a las pruebas. También implica que la experimentación es congruente con la ciencia.
- La lista de palabras de la definición de probar no es exhaustiva de todo lo que puede implicar probar, sino que representa los procesos mentales que consideramos más vitales y característicos.
- "algorítmico" significa que puede expresarse explícitamente de forma que una herramienta pueda realizarlo.
- "observaciones" pretende abarcar todo el proceso de observación, y no sólo el resultado.
- "observaciones específicas" significa que el proceso de observación da como resultado una cadena de bits (de lo contrario, las reglas algorítmicas de decisión no podrían operar sobre ellos).

Estas definiciones tienen ciertas implicaciones:

- Probar incluye la acción de checar (si es que existe), mientras que la acción de checar no puede incluir probar.
- Probar puede existir sin la acción de checar. Una prueba puede existir sin algún chequeo. Pero la acción de checar es una parte muy importante y popular del proceso de probar común, incluso del proceso más informal.
- Checar es un proceso que, en principio, puede realizar una herramienta en lugar de un ser humano, mientras que probar sólo puede ser asistido por herramientas. Sin embargo, las herramientas pueden servir para mucho más que checar.
- No estamos diciendo que un chequeo DEBE ser automatizado. Pero la característica definitoria de un chequeo es que puede automatizarse COMPLETAMENTE, mientras que las pruebas son intrínsecamente una actividad humana.
- Probar es una investigación abierta - pensemos en "Sherlock Holmes"-, mientras que la acción de checar es la abreviatura de "verificación de hechos" y se centra en hechos concretos y reglas relacionadas con esos hechos.
- Checar no es lo mismo que confirmar. Los chequeos se utilizan a menudo de forma confirmatoria (más típicamente durante las pruebas de regresión), pero también podemos imaginarlas como una forma de desconfirmación o de exploración especulativa (es decir, un conjunto de chequeos generados automáticamente que recorren aleatoriamente un vasto espacio en busca de algo diferente).
- Un problema común en nuestra industria es que checar se confunde con probar. Nuestro propósito aquí es reducir esa confusión.
- Un chequeo es descriptible; una prueba puede no serlo (porque, a diferencia de un chequeo, una prueba requiere un conocimiento tácito).
- Una afirmación, en el sentido de la Informática, es un tipo de chequeo. Pero no todos los chequeos son afirmaciones, y aún en el caso de las afirmaciones, puede haber código antes de la afirmación que forme parte del chequeo, pero no de la afirmación.
- Estas definiciones no son juicios morales. No estamos diciendo que checar sea algo intrínsecamente malo. Al contrario, puede ser muy importante. Lo que queremos decir es que para que el chequeo sea considerado bueno, debe producirse en el contexto de un proceso de pruebas adecuado. Checar es una táctica de las pruebas.

## Hacia donde va la sapiencia?

Si sigues nuestro trabajo, sabrás que hemos dado mucha importancia a la sapiencia. Un proceso sapiente es aquel que requiere un ser humano debidamente capacitado para llevarlo a cabo. Sin embargo, tras varios años de práctica con ese calificativo, nos hemos dado cuenta de que es casi imposible evitar dar la impresión de que un proceso no sapiente (es decir, uno que no requiere un humano pero que podría implicar, no obstante, a un humano con mucho talento y habilidad) es un proceso estúpido para gente estúpida.

Esto es porque la palabra sapiencia suena como inteligencia. Algunos de nuestros colegas se han opuesto rotundamente a que hablemos de procesos no sapientes basándonos en ese malentendido. Por lo tanto, creemos que ha llegado el momento de ofrecer a este término su reloj de oro y desearle lo mejor en su jubilación.

## Chequeos humanos vs Chequeos con máquinas

Aunque la sapiencia es problemática como etiqueta, seguimos necesitando distinguir entre lo que los humanos pueden hacer y lo que las herramientas pueden hacer. Por eso, además de la distinción básica entre checar y probar, también distinguimos entre chequeos humanos y chequeos con máquinas. Esto puede parecer un poco confuso al principio, porque checar es, por definición, algo que pueden hacer las máquinas. Se podría pensar que los chequeos humanos son lo mismo que los chequeos automáticos. Pero no es así. No puede serlo.

En los chequeos humanos, los humanos intentan seguir un proceso algorítmico específico. Sin embargo, en el caso de las herramientas, éstas no sólo siguen ese proceso, sino que lo encarnan. Los humanos no pueden encarnar ese algoritmo. He aquí un experimento mental para demostrarlo: dile a cualquier humano que siga una serie de instrucciones. Haz que esa persona acepte. Ahora observa lo que ocurre si haces imposible que esa persona siga las instrucciones. Los seres humanos no se quedarán ahí sentados hasta que mueran de sed o de exposición; se detendrán y cambiarán o abandonarán el proceso. Y es entonces cuando se sabe con certeza que ese ser humano, en todo momento, estaba encarnando algo más que el proceso que aceptó seguir e intentó seguir. Si hablamos de personas con una capacidad cognitiva normal, o incluso mínima, no hay vuelta de hoja. Sea cual sea el procedimiento que los humanos parecen seguir, siempre están haciendo algo más. Los humanos interpretan y ajustan constantemente sus acciones de un modo que las herramientas no pueden. Esto es inevitable.

Los humanos pueden realizar acciones con una *motivación*; las herramientas sólo pueden mostrar un *comportamiento* programado (véase el brillante libro de Harry Collins y Martin Kusch *The Shape of Actions*, para una explicación completa del por qué). En resumen: se puede definir un chequeo con bastante facilidad, pero un humano realizará al menos un poco más durante ese chequeo -y también menos en algunos aspectos- que una herramienta programada para ejecutar el mismo algoritmo.

Comprendamos por favor, debemos fomentar el rol de las herramientas en el proceso de probar. A medida que trabajamos hacia un futuro de un proceso de pruebas calificado, poderoso y eficiente, esto requiere una cuidadosa atención tanto al lado humano como al lado mecánico de la ecuación del proceso de pruebas. Las herramientas pueden ayudarnos de muchas maneras, mucho más allá de la automatización de los chequeos. Pero en esto, las herramientas desempeñan un papel de apoyo a las personas calificadas, y el uso no calificado de las herramientas puede tener consecuencias terribles.

<img src=":/assets/probarvschecar.PNG" width="804" height="551">

&nbsp;

También te preguntarás por qué no llamamos a los chequeos humanos simplemente " probar". Pues, sí lo hacemos. Ten en cuenta que todo esto ocurre en el ámbito del proceso de probar. Los chequeos humanos forman parte de probar. Sin embargo, pensamos que cuando los humanos intentan explícitamente limitar su pensamiento a los confines de un chequeo -aunque no lo consigan por completo- se trata ahora de una táctica específica y restringida de la prueba y no de toda la actividad de hacer pruebas. Merece una etiqueta propia dentro de lo que es probar.

Con todo esto en mente, y con el objetivo de aclarar confusiones, afinar nuestra percepción y fomentar la colaboración, recordemos nuestra definición de checar:

***Checar*** *es el proceso de hacer evaluaciones aplicando reglas de decisión algorítmicas a especificas observaciones de un producto.*

Así hemos identificado tres tipos de chequeos:

***Chequeos Humanos*** *es un proceso de comprobación en el que los humanos reúnen las observaciones y aplican las reglas sin la ayuda de herramientas.*

***Chequeos Mecánicos*** *es un proceso de comprobación en el que determinadas herramientas recopilan las observaciones y aplican las reglas sin intervención humana.*

***Chequeos hombre/máquina*** *es un intento del proceso de checar en el que humanos y herramientas interactúan para recoger las observaciones y aplicar las reglas.*

Para explicarlo en profundidad, tendremos que hablar de ejemplos concretos. Los encontrarás en un próximo artículo.

Mientras tanto, te invitamos a hacer comentarios al respecto.