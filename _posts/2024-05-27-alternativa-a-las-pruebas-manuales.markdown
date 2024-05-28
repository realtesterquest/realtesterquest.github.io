_Esta es una traducción del post titulado “Alternatives to “Manual Testing”: Experiential, Interactive, Exploratory” que puedes encontrar en el sitio de Michael Bolton_

[https://developsense.com/blog/2021/08/alternatives-to-manual-testing-experiential-attended-exploratory](https://developsense.com/blog/2021/08/alternatives-to-manual-testing-experiential-attended-exploratory)

_Al hacer esta traducción intente utilizar un Español lo mas neutral posible pero no puedo garantizar el resultado, así que antes de mandarme a la Inquisición recomiendo leer el post original o podemos tener una conversación sobre el mismo, enviame un correo a andres@testerquest.ca._


# **Alternativas a las "Pruebas Manuales": Experiencial, Interactiva, Exploratoria**

_Esta es una extensión de un largo debate en Twitter de hace un tiempo que llegó a LinkedIn, pero no a mi blog._

_Actualización, 2022/12/07: James Bach y yo hemos cambiado recientemente "asistida" por "interactiva", para enfatizar la interacción directa del tester con el producto que se lleva a cabo durante las llamadas pruebas "manuales". "Interactivo" es más indicativo de lo que ocurre que "asistido", pero también es cierto que la interacción del tester puede limitarse a observar lo que ocurre en el preciso momento. He cambiado este post (y su título) para reflejarlo._

Los testers que se toman el testing en serio tienen problemas para que la gente entienda lo que es testing.

El problema es un caso especial que rodea cualquier aspecto de la experiencia humana entre los que están adentro y los que están afuera : la mayoría de las veces, los que están afuera de un grupo social -una comunidad, una cultura, un grupo de personas con cierta experiencia, un país, un club de fans- no entienden la perspectiva de los que están adentro. Los de adentro tampoco entienden la perspectiva de los que están afuera.

No sabemos lo que no sabemos. Esto debería ser obvio, por supuesto, pero cuando no sabemos algo, no tenemos ni idea de lo poco que lo comprendemos, y nuestra experiencia y nuestra falta de experiencia pueden llevarnos por un mal camino. "¡Conducir es fácil! Sólo tienes que meter la velocidad y arrancar". Probablemente eso funcione muy bien en cualquiera que sea tu contexto actual. Ahora te invito a que te pongas detrás del volante en Bangalore.

¿Qué relación tiene esto con testing? Aquí lo explicamos:

_Nunca nadie se sienta delante de una computadora y compila accidentalmente un programa que funcione, por lo que la gente sabe -de manera intuitiva y correcta- que programar debe ser difícil._

_En cambio, casi cualquiera puede sentarse delante de una computadora y toparse con bugs, por lo que la gente cree -de forma intuitiva e **incorrecta**- que testing debe ser fácil._

En nuestro mundo de desarrollo de software, existe la fantasía de que si todo el mundo tiene buena voluntad y se esfuerza mucho, todo saldrá bien. Si creemos en esa fantasía, no necesitamos buscar profundos, ocultos, raros, sutiles, intermitentes y emergentes problemas; la buena voluntad de la gente los hará mágicamente imposibles. Es, por decirlo con delicadeza, un enfoque muy optimista del riesgo. Está bien para productos que no son muy importantes. Pero si nuestros productos importan, corresponde a nosotros buscar problemas. Y para encontrar problemas profundos de forma intencionada, ayuda mucho contar con testers calificados.

Sin embargo, el papel del tester no siempre es bienvenido. El problema es que para crear un producto novedoso y complejo se necesita una enorme dosis de optimismo, una actitud de "sí se puede". Pero como me dijo una vez mi amiga Fiona Charles -parafraseando a Tom DeMarco y Tim Lister- en un entorno de “sí se puede”, la gestión del riesgo se "criminaliza". Yo iría más lejos: en un entorno de "sí se puede", incluso el _reconocimiento_ del riesgo está penalizado.

En[ Waltzing With Bears](https://www.oreilly.com/library/view/waltzing-with-bears/9780133492248/), DeMarco y Lister señalan: "El resultado directo de "sí se puede" es poner freno a cualquier tipo de análisis que sugiera "no se puede"... Cuando se establece una estructura de administración de riesgos, se autoriza a la gente a pensar negativamente, al menos parte del tiempo. Las empresas que lo hacen entienden que el pensamiento negativo es la única forma de evitar que el riesgo nos sorprenda a medida que avanza el proyecto."

La negación al riesgo se desarrolla en un documental maravilloso, "[General Magic](https://www.generalmagicthemovie.com/)", acerca de una tienda de desarrollo de software del mismo nombre. En los primeros años de la década de los 90 's (¡impresionante!), General Magic trabajaba en un dispositivo que, en términos de capacidad, diseño y ambición, era virtualmente similar al iPhone que fue lanzado unos 15 años después.

La película vale mucho la pena. En uno de los segmentos,[ Marc Porat](https://en.wikipedia.org/wiki/Marc_Porat), el líder del proyecto, habla en retrospectiva sobre por qué General Magic fracasó sin siquiera acercarse al lanzamiento del producto. Él dice: "Había confianza total y una seguridad absoluta; ninguna duda de '¿Podría estar equivocado?'. Ninguna... Eso es lo que necesitas para escapar de la gravedad de la Tierra. Necesitas algo que te permita liberarte de la atracción terrestre. Necesitas una gran cantidad de impulso... que proviene de silenciar tus dudas sobre la posibilidad de fracasar.

Esa forma de pensar persiste en todo el desarrollo de software, incluso hasta el día de hoy. Como profesión, el negocio del desarrollo de software sistemáticamente se resiste a pensar críticamente sobre problemas y riesgos. Desafortunadamente para los testers, ese es el área en el que habitan.

Los developers tienen una gran habilidad, experiencia y conocimiento tácito en conectar el mundo de las personas y el mundo de las máquinas. Lo que tienden a no tener - y casi todo el mundo es igual, no solo los programadores - es la inclinación de encontrar problemas. Al developer le interesa hacer desaparecer los problemas de la gente. Los testers tienen el difícil trabajo social de encontrar y reportar sobre los problemas allá donde miren. A diferencia de cualquier otra persona en el proyecto, los testers se centran en revelar problemas que no están resueltos o problemas introducidos por nuestra solución propuesta. Es un aspecto al que los constructores, por naturaleza, suelen resistirse.

La resistencia a pensar sobre los problemas se manifiesta en muchas ideas inútiles y falsas. Algunas personas creen que el único tipo de error es un error de codificación. Algunos piensan que lo único que importa es cumplir con las intenciones de los constructores para el producto. Otros están convencidos de que podemos encontrar todos los problemas importantes en un producto escribiendo chequeos mecanizados del mismo. Estas ideas reflejan los sesgos naturales del constructor, el optimista. Estas ideas hacen posible imaginar que testing se puede automatizar.

La idea falsa y poco útil de que testing se puede automatizar lleva a dividir las pruebas en "pruebas manuales" y "pruebas automatizadas".

Escucha: ningún otro aspecto del desarrollo de software (o de hecho de cualquier trabajo social humano, cognitivo, intelectual, crítico, analítico o investigativo) se divide de esa manera. No hay "programadores manuales". No existe "investigación automatizada". Los gerentes no gestionan proyectos manualmente y no existe la "gestión automatizada". Los médicos pueden utilizar herramientas muy potentes y sofisticadas, pero no hay "médicos automatizados", ni existen los "médicos manuales" y ningún médico aceptaría ni por un minuto ser clasificado de esa manera.

[Testing no se puede automatizar. Ok, punto](http://www.satisfice.com/blog/archives/856). Ciertas tareas dentro y alrededor del testing pueden beneficiarse mucho de las herramientas, pero utilizar maquinaria para presionar teclas virtuales y comparar la salida del producto con la especificada no es más "pruebas automatizadas" que el corrector ortográfico es "edición automatizada". Basta de todo eso, por favor.

Es poco útil agrupar todas las tareas no mecánicas de testing bajo "pruebas manuales". Hacerlo es como referirse a los aspectos artesanales, sociales, culturales, estéticos, químicos, nutricionales o económicos de cocinar como "cocinar a mano". Nadie que proporcione alimentos con cuidado y preocupación por el bienestar humano - o incluso animal- sugeriría que todo lo que importa en la cocina son los procesadores de alimentos, los hornos de microondas y las licuadoras. Por favor.


## **Términos más precisos para “pruebas manuales”**

Si quieres comprender el estado de tu producto, probablemente quieras probarlo. Querrás que la prueba te diga si el producto que tienes es el producto que deseas. Si te importa eso, necesitas entender algunas cosas importantes sobre lo que es testing.

Si quieres entender cosas importantes sobre testing, querrás considerar algunas cosas que comúnmente se pasan por alto con la frase "pruebas manuales". Considerarlas podría requerir nombrar algunos aspectos de testing que no has mencionado antes.


### **Testing experencial**

Pensando en el testing experiencial, donde el tester interactúa con el producto y las acciones que realiza el tester son como las que haria un usuario. ¿No es verdad que un producto no es solo su código ni los objetos virtuales en una pantalla? Un producto de software es la experiencia que proporciona a las personas al intentar lograr algo, satisfacer un deseo, disfrutar de un juego, ganar dinero, conversar con personas, obtener un préstamo hipotecario, aprender nuevas cosas o salir de prisión...

Contrastemos la prueba experiencial con la prueba instrumental. La prueba instrumental es la que se efectúa a través de un medio (algunas herramientas, tecnologías o mecanismos) que se interpone entre el tester y la experiencia natural con y del producto. La instrumentación altera, acelera o distorsiona; en ciertos aspectos lo hace de manera útil, pero en otros no tanto. Debemos mantenernos conscientes de los efectos, tanto deseables como indeseables, que la instrumentación aporta a nuestro testing.


### **Testing Interactivo**

Estás diciendo "pruebas manuales"? Podrías estar refiriéndote a los aspectos interactivos, asistidos o comprometidos de las pruebas. En ese modo, el tester está directamente y inmediatamente observando y analizando aspectos del producto y su comportamiento en el momento mismo en que ocurre el comportamiento. El tester puede estar controlando el producto, ya sea de manera directa a través de la interfaz de usuario o indirectamente mediante algún tipo de herramienta.

Habiendo notado que hay momentos en que observas e interactúas con el producto, podrías querer contrastar eso con el testing que no requiere tu presencia inmediata o control. Algunas tareas pueden ser manejadas por cosas algorítmicas y mecánicas que las máquinas pueden hacer sin asistencia. Algunas de estas son cosas que algunas personas etiquetan como "pruebas automatizadas" - excepto que la prueba no puede ser automatizada. Una prueba requiere de el diseño antes del comportamiento automático, y la interpretación después. Aquellas partes de la prueba, que dependen de la competencia social humana para hacer un juicio, no pueden ser automatizadas.


### **Testing Exploratorio**

Estás diciendo "manual"? Podrías estar refiriéndote al trabajo exploratorio, que es notablemente distinto del trabajo experiencial descrito anteriormente. Exploratorio—en el ámbito de Rapid Software Testing —[se refiere a la agencia](http://www.satisfice.com/blog/archives/1509) (autoridad); de quién o qué está a cargo de hacer elecciones sobre testing.[ Hay más información disponible sobre este tema.](http://www.satisfice.com/blog/archives/1509).


### **Espera... ¿No son lo mismo la prueba experiencial y la prueba exploratoria?**

Podrías estar explorando—haciendo elecciones sin un script—de manera enteramente distinta de la forma en que el usuario normalmente utilizaría al producto. Podrías generar montañas de datos e interactuar con el producto para estresarlo; o podrías estar explorando mientras intentas privar al producto de recursos. Podrías realizar una acción y luego analizar los datos producidos por el producto para encontrar problemas, en cada momento manteniendo el control sobre tus decisiones sin ser controlado por un script o un procedimiento.

Es decir, podrías estar explorando mientras utilizas el producto para investigarlo. Eso es algo genial, pero eso es utilizar el producto como un tester, en lugar de como un usuario. Podría ser una idea excelente ser consciente de las diferencias entre estos dos aspectos y aprovecharlas, pero no confundirlas.

Podrías estar haciendo pruebas experienciales de una forma muy programada, mucho menos exploratoria. Por ejemplo, podrías seguir un tutorial orientado al usuario y recorrer cada uno de sus pasos para observar las inconsistencias entre el tutorial y el comportamiento del producto. Para alguien externo, tu interacción se parecería bastante a la de un usuario; esta persona te vería interactuando con el producto de forma natural, en la mayoría de los casos, excepto en los momentos en los que registras observaciones, errores, problemas, riesgos e ideas de pruebas. Pero la mayoría de los observadores ajenos a la forma de vida del tester no notarán esos momentos.

Claro que hay coincidencias entre estos dos tipos de interacciones. Una diferencia clave es que el tester, al encontrar un problema, lo investiga y lo comunica. Es mucho menos probable que un usuario lo haga. ( Nótese este fenómeno, al intentar introducir un enlace desde el editor de artículos de LinkedIn; el botón "aplicar" no está visible, y se esconde en la parte derecha del popup. Me dí cuenta de esto mientras interactuaba con LinkedIn de forma experiencial. Me gustaría pensar que también habría encontrado este problema al probarlo intencionadamente, de forma exploratoria).


### **Testing transformativo**

¿Estás diciendo "manual"? Es posible que te refieras a una actividad de prueba que es transformativa, en donde algo sobre la ejecución de la prueba cambia al tester en algún sentido. Las pruebas transformativas tienen que ver con el aprendizaje, el desarrollo de inspiración, la identificación de riesgos o la generación de ideas para el diseño de pruebas. En las primeras fases del testing, especialmente, puede ser muy importante relajar o suspender nuestro enfoque en la búsqueda de problemas y prestar más atención a la construcción de nuestros modelos mentales del producto. Eso allana el camino para hacer pruebas más profundas más adelante.

Contrasta este modo de realizar pruebas con otro muy procedimental: las pruebas transaccionales que consisten en marcar casillas de forma rutinaria. La mayoría de las cosas transaccionales pueden hacerse mecánicamente. Las máquinas no se ven realmente afectadas por lo que ocurre y no aprenden en ningún sentido significativo. Los humanos sí, y tenemos que aprender el producto en profundidad si queremos encontrar los bugs profundos.

Sin duda, existen otras dimensiones de las "pruebas manuales". Durante un tiempo, consideramos que las "pruebas especulativas" eran algo a lo que la gente se refería cuando hablaba de "pruebas manuales"; "¿y si...?". Lo comparamos con las pruebas "demostrativas", pero luego pensamos que la demostración no es realmente una prueba. Al menos, no pretende serlo. Para que una acción sea una prueba, tenemos que ser especulativos por naturaleza.


### **Testing manual es ... Testing**

Esto es lo más importante: si eres un "tester manual", estás haciendo testing todo el tiempo. Si eres un "tester automatizado", o un "ingeniero de automatización", también estás haciendo enormes cantidades de "pruebas manuales" todo el tiempo - a menos que simplemente estés escribiendo chequeos automatizados para alguna especificación, ejecutándolos, e ignorando completamente los resultados.

Los testers son alimentados con mierda de manera frecuente. Una porción de la mierda viene en un plato que dice que las pruebas "automatizadas" son de alguna manera "mejores" que las pruebas "manuales". Pero no puedes afirmar que estás haciendo testing a menos que estés experimentando, explorando e interactuando con un producto a través de experimentos. (En este caso, el "producto" puede ser un software en funcionamiento o algún componente del mismo. Pero también puede ser una maqueta, un diseño, un dibujo, la descripción de una idea; esas cosas se pueden probar experimentándolas, explorándolas y experimentando con ellas en tu mente). Las herramientas pueden proporcionar un apoyo inmenso para ese tipo de trabajo, pero caracterizar las pruebas como "automatizadas" es ignorar todo lo que no implique a la maquinaria.

Se afirma que las "pruebas manuales" son lentas y propensas a errores, como si no se cometieran errores al automatizar los chequeos. Lo hacen, y la automatización facilita esos errores a una escala mucho mayor y más rápida.

Claro que los chequeos automatizados son rápidos y tienen un bajo costo de ejecución. Pero pueden tener un costo de desarrollo elevado, un costo de mantenimiento enorme, un costo de interpretación muy elevado (averiguar qué ha fallado puede llevar mucho trabajo) y un costo de transferencia elevado (explicarlas a quienes no las han escrito).

Hay otro costo, relacionado con estos otros. Está muy bien escondido y no se tiene en cuenta: podríamos llamarlo costo de interpretación o costo de análisis. Un grupo de chequeos automatizados lo suficientemente grande es impenetrable; no se puede comprender sin una revisión muy costosa. ¿Los chequeos que siempre están en verde sirven para algo? Quién sabe... a menos que entres en un proceso "manual" y evalúes lo que estás observando.

Los chequeos en rojo reciben atención con frecuencia, pero muchos de ellos son, ya sabes, "poco confiables"; deberían estar en verde cuando en realidad están en rojo. De los miles que están en verde, ¿cuántos deberían estar en rojo? Saberlo es costoso desde el punto de vista cognitivo, así que la gente los ignora sistemáticamente.

Y todos estos costos representan otro costo oculto: el costo de oportunidad; el costo de hacer algo tal que nos impide hacer otras cosas igual o más valiosas. Ese costo es inmenso, porque lleva mucho tiempo y esfuerzo automatizar comportamientos en interfaces gráficas de usuario cuando podríamos estar interactuando directamente con el maldito producto.

Y está ocurriendo algo aún más extraño: en lugar de enseñar a los testers no técnicos a programar y adquirir una experiencia natural con las API, los ponemos frente a interfaces gráficas de las API. Así que tenemos a programadores especializados intentando automatizar las interfaces gráficas y, al mismo tiempo, a testers no programadores que utilizan Cypress para evitar la experiencia de uso de las API. La experiencia del tester de una API a través de Cypress es enormemente diferente de la experiencia del programador al intentar utilizar la API.

Y no se anima a ninguno de estos testers a analizar el costo y el valor de los métodos que adoptan. El tecnochauvinismo (gran palabra; léase el libro de Meredith Broussard[ Artificial Unintelligence](https://mitpress.mit.edu/9780262537018/artificial-unintelligence/)) refuerza la ilusión de que probar el software es una tarea rutinaria, mecánica, como de fábrica, que sólo espera ser programada. Esto es falso. Las pruebas pueden beneficiarse de las herramientas, pero no pueden mecanizarse.

Testing tiene que centrarse en encontrar problemas que perjudiquen a las personas o las hagan infelices. ¿Por qué? Porque los optimistas que construyen un producto tienden a no ser conscientes de los problemas, y esos problemas pueden esconderse en el producto. Cuando los constructores son conscientes de esos problemas, pueden afrontarlos. Así quedan bien, ganan dinero y ayudan a la gente a vivir mejor.

Testing tiene que considerarse un oficio social (y socialmente desafiante), cognitivo, centrado en el riesgo, crítico (en varios sentidos), analítico, investigador, hábil, técnico, exploratorio, experiencial, experimental, científico, revelador y honorable. No "manual" ni "automatizado". Exijamos a esa distinción engañosa que se tome unas largas vacaciones en una isla desierta hasta que muera de abandono.
