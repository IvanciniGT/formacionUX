# UI

## Cuestiones a considerar en UI

- Diseño estético => QUE REFUERCE la usability y la ux
  - Acceder/identificar/entender la información que representamos
- Rendimiento => Usability y UX
  - Especialmente en el mundo WEB
- Robusto. Que se pueda utilizar desde distintos DISPOSITIVOS/HERRAMIENTAS (responsive)
- Accesibilidad
- Comunicar información del estado del sistema (FEEDBACK... )
  - Cuando doy a un botón
  - Animaciones, barras de progreso, Efectos visuales

## Principios generales de diseño de interfaces

### Consistencia visual y funcional

  Toda lo que representemos en la UI debe ser coherente a lo largo de nuestro sistema:
    - Tipografía
    - Esquemas de color
    - Formas de botones
    - Enlaces
    - Respuestas a eventos

### Jerarquía VISUAL <<< CRITICO (La definimos a nivel de Usabilidad)

### Espaciado y simetría

Queremos interfaces: 
- Limpias / Organizada (Jerarquía visual)

### Color y contraste

- Identidad de marca
- El cómo afecta esto a:
  - Legibilidad (contrastes) / Accesibilidad
  - Emociones (satisfacción,...)
  - Jerarquías visuales
  - Intenciones (BOTON CONTINUAR | BOTON CANCELAR) BOTONES PRIMARIOS / SECUNDARIOS

### Tipografía

En muchos entornos, las tipografías están totalmente especificadas. Y las sigo.
En contenidos (WEB), puedo tener más libertad.

Aspectos a tener en cuenta:
- Legibilidad
- Accesibilidad
- Jerarquía visual

Distintos tipos de fuentes:
- Sans-serif Hay fuentes hoy en día Sans-serif que son muy legibles y ofrecen un aspecto más moderno
- Serif      En general las fuentes serif se consideran más legibles (libros, periódicos)
- Script:    Puramente estético (logo). Sólo las usamos para un uso funcional en casos muy concretos: Un quote (recomendación, una cita, El nombre de una persona que firma algo)
- Monospace: Para código / algo que emule una máquina de escribir (guión de una película)

### Simplicidad -> Minimalismo (Menos es más - KISS [Keep it simple, stupid], YAGNI [You aren't gonna need it])

La menos información y ruido posible en la UI.

- Si pongo una imagen es porque aporta valor a la información que quiero transmitir.
- No pongo más datos de los que necesito (Tiendo a esconder datos que no son necesarios o al menos no lo son en primera instancia)

### Retroalimentación / Feedback

El usuario necesita saber que le hemos entendido y que estamos trabajando en ello:
- hover
- click
- loading
- efectos
- animaciones

Puedo intentar además, convertir esto en una experiencia positiva para el usuario!
- Puedo hacer que al responder a una pregunta de un examen, se ponga algo en verde o rojo. FRIO
- Puedo hacer que le salgan unas estrellitas en la pantalla! GENERA EMOCIONES (ENDORFINAS)
- TIK-TOK: Me ponen en la pantalla que cuando aprieto encima del video para un like: Me sale un festival de emoticonos en la pantalla...
  Y además voy viendo las reacciones que va marcando todo el mundo. (ENDORFINAS) -> ADICCION

### Iconografía clara y familiar

No me invento iconos. Uso los que ya existen y que son conocidos por el usuario.

Antiguamente tirábamos mucho para las apps desktop de librerías de iconos custom (que eran una rayada)

Estilos de iconos:
- Flat
- Material Design
- 3D

### Responsive design

- Que se vea bien en cualquier dispositivo
- Y que aproveche las características/espacio de cada uno de ellos

### No fliparnos con la creatividad

- Animaciones moderadas
- Transiciones suaves

### La UI tiene que ir TOTALMENTE ALINEADA CON LA USABILIDAD / UX

### Facilidad de uso

Que sea intuitivo. Que el usuario no tenga que pensar mucho para entender cómo funciona.

---

En muchos formularios, tendemos a poner GUARDAR y Cancelar, uno al lado del otro. Esto es una costumbre (heredada de windows), que puede tener sentido en ciertas interfaces.. pero no en todas.
- Si me abres un modal en Windows para un aviso... El modal es chiquito... y pondrás todos los botones juntos.

En un e-commerce... ni de coña.

---

# Rendimiento en el mundo WEB:

En el mundo WEB lidiamos con contenidos de gran tamaño.
Tenemos que tener esto en cuenta:
- Imágenes: Quiero las imágenes de un tamaño exacto. No quiero que el navegador tenga que hacer un resize de la imagen.
    Ni hacía arriba (Mostrar la imagen más grande de lo que estoy mandando (tengo una pérdida de calidad))
    Ni hacía abajo (Me mandas una imagen más grande de lo que necesito y la tengo que hacer más pequeña)
    Si quiero ver una ampliación de la imagen.. ya me la mandas ampliada.
    - También aplicamos técnicas de:
      - Carga asíncrona de imágenes
      - Carga inicial en baja resolución
- Carga de scripts
    Una cosa son los scripts que montamos nosotros... y otra los que usan nuestros scripts (dependencias)
        Angular, React, Vue, etc... Los scripts son grandes.
    Técnicas:
        - Minificación: Eliminar espacios en blanco, comentarios, etc...
                        Cambiar nombres de variables a nombres más cortos
                        Union de archivos (js)
        - Cargas asíncronas
En mi página, me aseguro de que en carga inicial, ya haya algo representable en pantalla.. Y el resto... ya vendrá.

- Caches. Queremos un HTML muy limpio:
  - Estilos        CSS  \
  - Funcionalidad: JS   / Los queremos cacheables a nivel del navegador

Si tengo una página que tiene una parte dinámica... y otra que no: ARTICULO DE UN BLOG.
- Lo que es el artículo en sí, no cambia. Lo puedo cachear.
- Los comentarios, si cambian. No los cachearé.

Si devuelvo un único HTML tengo problemas, necesito mandar todo de nuevo.
Si el HTML inicial la parte de los comentarios la carga dinámicamente, puedo cachear el HTML inicial (que contiene el artículo) y luego cargar los comentarios dinámicamente JS.

- WORDPRESS: Está un poquito obsoleto (PHP). Usamos sistemas de cache... pero van a medio gas.

---

# JERARQUIA DE NORMAS Y PRINCIPIOS A APLICAR

## Experiencia de usuario (UX)
  ^^
## Usabilidad
  ^^
## UI
  ^^
## Principios generales de diseño de interfaces
  ^^
## Guías específicas para el diseño de interfaces (dependiendo del tipo de aplicación / dispositivo)
  ^^
## Guías de diseño de interfaces a nivel corporativo (ESTILOS)

---

## ACCESIBILIDAD

El concepto de accesibilidad se refiere a garantizar que todos los tipos de usuarios que voy a tener un un sistema puedan hacer un uso efectivo y eficiente de él.

En ocasiones, el tipo de app que estamos montando tiene un espectro de usuarios muy limitado:
- Simulador de una cabina de un avión.

En ocasiones, el espectro de usuarios es muy amplio:
- Cualquier App. Mobile, web, muchas desktop.
- Más aún si pertenece a un organismo público.
- Pero aún pertenece a una empresa privada, existen leyes que obligan a que la app sea accesible.

Lo primero es entender los tipos de necesidades especiales que pueden tener los usuarios:
- Discapacidades visuales:
  - Visión reducida
  - Ceguera total
  - Daltonismo
- Discapacidades auditivas: 
  - Sordez total: Todo lo que sea contenido multimedia: AUDIO -> SUBTITULOS / TRANSCRIPCIONES
      - Eventos online: Subtitulos en directo
      - Eventos en diferido: Subtitulos + Transcripciones
- Discapacidades motoras:
  - Movilidad limitada manos, brazos
    - Parkinson
    - Artritis/Artrosis
  - Pérdida de extremidades
- Discapacidades cognitivas:
  - Dificultades de aprendizaje
  - Problemas de memoria
  - Deficiencias de atención (TDAH) <<< RRSS es un problema
  - Personas con un nivel cultural bajo
- Sensibilidad a la luz:
  - Leve (como el mío) - Cada vez más apps y sitios web incluyen la opción de modo oscuro (SO: Windows/MacOS/iOS/Android)
  - Grave: Crisis epilépticas

En este sentido, tenemos 2 grandes guías:

# WCAG (Web Content Accessibility Guidelines) <- W3C

4 principios fundamentales:

##  Perceptible:

Los elementos de la UI deben representarse de tal forma que cualquier usuario pueda PERCEPTIBLES / interpretarlos / "interactuar" con ellos.
- Necesitamos alternativas de texto para imágenes/videos/audios (problemas de visión y de audición)
- Contraste de color suficiente fondo/primer plano
- Capacidad de ajuste: Aumento de fuente (MUCHO DE ESTO me lo ofrecen ya las plataformas: CHROME, EDGE, FIREFOX, SAFARI, WINDOWS, MACOS, IOS, ANDROID)

## Operable:

Hace referencia a que los componentes de la interfaz gráfica (navegación, botones, etc...) deben ser operables por cualquier usuario, independientemente del medio que utilice para interactuar con la interfaz.

- No puedo depender de un ratón (Ni el dedo en la pantalla) <- TOOL TIP (que antes se usaba para explicar lo que hacía un botón)
    Podemos usar tooltips para explicar lo que hace un botón... pero no puedo depender del tooltip para que el usuario sepa que tiene que hacer click en un botón.
- Dar tiempo suficiente para las acciones (TOAST, MENSAJES TEMPORALES, ANIMACIONES QUE APORTEN VALOR)
- Evitar contenidos/animaciones/estética que puedan causar crisis (no más de 3 parpadeos por segundo)
- Elementos de navegación claros y consistentes (personas con problemas cognitivos /dificultades motoras)
    Puede ser que mi web la haya montado para poder saltar con el TABULADOR DEL TECLADO DE UNA SECCION A OTRA
    USAR LAS ETIQUETAS SEMANTICAS DE HTML5 (NAV, HEADER, FOOTER, ASIDE, MAIN, ARTICLE, SECTION, LABEL) 
        Esas etiquetas son procesadas por los programas de ayuda a usuarios con necesidades especiales <- EFICIENCIA

## Comprensible:

La información / navegación / interfaz debe ser comprensible para cualquier usuario.
- Texto legible y comprensible, en un lenguaje claro y sencillo
   ACRONIMOS (ofrecer la posibilidad de ver el significado de un acrónimo)
- Componentes de la interfaz coherentes y predecibles
- Asistencias en la introducción de datos SUGERENCIAS, ejemplos (PLACEHOLDERS) + validaciones en tiempo real
    NOTA: Los placeholders no son un sustituto de las etiquetas (label) de los campos de un formulario
                                                                  ^
                                                                  etiqueta semántica

RUINA = MIERDA desde el punto de vista de accesibilidad... Podrá quedar bonito... YO PODRE ENTENDERLO... pero no es accesible.
```html
     <div class="form-section>
        <div class="single-row-text-field">
            <span class="field-title>Nombre</span>
            <input type="text" id="nombre" name="nombre">
        </div>
    </div>
``````html
     <div class="form-section>
        <div class="single-row-text-field">
            <input type="text" id="nombre" name="nombre" placeholder="Inserte su nombre">
        </div>
    </div>
```

GUAY
```html
     <div class="form-section>
        <div class="single-row-text-field">
            <label for="nombre">Nombre</label>
            <input type="text" id="nombre" name="nombre" tabindex="1" placeholder="John Doe">
        </div>
    </div>
```

## Robusto

- Compatibilidad con tecnologías de asistencia (1)
- Compatibilidad con navegadores
- Seguir estándares actualizados (1)


## Directrices de Accesibilidad WCAG

Las recomendaciones concretas que hace el WCAG para cumplir con los 4 principios fundamentales se clasifican en 3 niveles de conformidad:

- A: Mínimo necesario para que un sitio web sea considerado accesible
- AA: Accesibilidad deseable para la mayoría de los sitios web que ofrece una experiencia mejorada para los usuarios con discapacidades
      - Relación de contraste 4,5:1
- AAA: Nivel más alto de accesibilidad, que garantiza una experiencia óptima para todos los usuarios
      - Relación de contraste 7:1

    Reacción de contraste lo que toma es el color más brillante (emisión percibida de luz de un elemento) y el color más oscuro y hace la división.

---

W3C: Una organización creada por Tim Berners-Lee (Creador de la WWW) para estandarizar la web:
- HTML
- CSS
- XML
- SVG
- WCAG

---

La accesibilidad es un tema que hasta cierto punto es muy cuantifiable!
Puedo tener test BASTANTE AUTOMATIZADOS para comprobar si mi web es accesible o no: A, AA, AAA

El tema de la usabilidad y la UX es más subjetivo.

Según subo de nivel... más subjetivo.
 
 UX                 MUY SUBJETIVO
 ^^
 Usabilidad
 ^^
 UI
 ^^
Accesibilidad       MUCHO MENOS SUBJETIVO <- TEST AUTOMATIZADOS

---

Para poder optimizar la usabilidad y la experiencia de usuario de mi web, o de mi app es necesario tener DATOS.

Hay 3 concepto que medidos:
- Eficacia          MUY OBJETIVO (TOTALMENTE OBJETIVO): Si el usuario consigue hacer lo que quiere hacer
                       Este dto(variable que mido) vale TRUE o FALSE 
- Eficiencia        NO ESTA OBJETIVO: Si el usuario consigue hacer lo que quiere hacer en un tiempo adecuado
                      ¿Qué es un tiempo adecuado? YO QUE SE! 
                      Aquí estoy con una variable cuantitativa de intervalo (No hay un cero absoluto)
                      - Puedo ver si un cambio que haga, o una decisión, mejora o empeora la eficiencia (el tiempo que tarda en hacer algo)
                      - Puedo definir unos límites absolutos (tiempo máximo que puede tardar en hacer algo). PERO SON SUBJETIVOS.
- Satisfacción      NADA OBJETIVO: TOTALMENTE SUBJETIVO
                      Variable medida en escala ordinal
                            ¿Cuál es tu grado de satisfacción? No la puedo medir con 1 punto o 7 puntos 
                                Lo que para un usuario es un 5, no es lo mismo que lo que ese 5 es para otro usuario.
                                    0-10
                      POCO---> MUCHO
                      Y eso implica que cuando trabajo luego con esa variable, puedo aplicar solo ciertas técnicas estadísticas: No puedo hacer una media!
                      NO SE PUEDE CONCEPTUALMENTE CALCULAR LA MEDIA DE SATISFACCIÓN DE LOS USUARIOS DE UNA APP
                      Puedo calcular la mediana !

---
El objetivo es crear un sistema que ofrezca una "buena" experiencia de usuario, que sea fácil de usar y que sea accesible para todos los usuarios.

Necesitamos COMPARAR!

---

# Diseño de test de usabilidad

Es clave... necesito datos.

- Definir los objetivos del test... Qué aspectos voy a medir
- Que recursos tengo (usuarios/expertos)
- Diseño de tareas
- Observación
- Análisis de resultados

## Métricas de usabilidad

- Tasa de éxito: % de tareas completadas con éxito                      \
                 % de usuarios que completan una tarea con éxito         > Lo ideal es poder comparar
- Número de errores hasta éxito                                         /
- Tiempo que tardamos en la tarea: COMPARATIVAS
- Satisfacción del usuario: COMPARATIVA

---

## Opción 1: 
El ocasiones no tengo opción de usuarios. En la industria se aplican mucho los test Heurísticos, que son test que se hacen con expertos.

- Se suelen tomar de referencia los 10 principios(heurísticas) de Nielsen, sirven de guía para las mediciones. PUEDO AJUSTARLOS A MI PROYECTO
- Elegir un grupo de expertos (3-5) que evaluarán la interfaz de forma independiente en cada uno de los principios
- Voy recopilando los problemas que van identificando los expertos
- Analizo los resultados y priorizo los problemas

Ideal si estoy además lo hago con algo con lo que puedo comparar.

Este tipo de test:
- Son baratos
- Dependen de la experiencia de los expertos (criterio)
- Pueden pasar por alto problemas que los usuarios tendrán

---

## Opción 2: Test con usuarios: ESTO ES LO MEJOR

Tengo que tener en cuenta que:
- Son caros y más complejos de poder realizarse
- Hay un problema adicional y que el grupo de usuarios sea representativo (PROBLEMA)
  Un grupo representativo no significa un grupo con todo tipo de personas.
  Un grupo representativo es un grupo con todo tipo de personas, en los % en los que se encuentran en la población general.
    Voy a poner a una Paula, a un Kevin, a una Gertu y a un Ramón y a un Teófilo
    Claro.. quizás Gertru y teo están fallando mucho en ciertas cosas.
    Y eso me lleva a pensar que tengo que meter mis esfuerzos (pasta, recursos, tiempo) en esas cosas...
    Pero resulta que en la realidad usuarios como Gertru y Teo son el 5% de mi población.
    Oye.. Gertru y Teo están guays... y trataré de que tengan buena experiencia.. Pero quizás antes intentaré que el 95% de mi población la tenga

---

Hay test mucho más especiales... orientados a cosas muy concretas:
- Pruebas de eye-tracking                       PRUEBA          \
- Pruebas de mapas de calor (mouse tracking)    MONITORIZACION  / Mejorar la estructura y la disposición de los elementos

Estas son mucho más caras y complejas de realizar (pueden requerir de equipos especializados, o programas de software específicos)
Pero son muchísimo más efectivas. Algunas de ellas, ni siquiera son pruebas... ya entran dentro del apartado MONITORIZACIÓN


ALIEXPRESS, según voy haciendo scroll con el dedito en la pantalla, va analizando donde me detengo... qué producto al menos estoy dedicando tiempo a mirar. Y van generando estadísticas en tiempo real... y van optimizando mi experiencia... SACANDO PRODUCTOS QUE ME INTERESAN MAS CADA VEZ
                                                                                 y su rentabilidad