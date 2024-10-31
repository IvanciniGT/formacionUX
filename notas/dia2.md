# Paso 1: Casos de Uso (Necesidades): También hay un estándar: Unified Modeling Language
# Paso 2: User PERSONAS
- Entender a mis usuarios
- Empatizar con mis usuarios
- Diseñar procesos que optimicen la experiencia de mis usuarios
- De cada USER PERSONA:
  - Nombre y Apellidos
  - Foto
  - Datos demográficos
  - Objetivo
  - Motivaciones
  - Puntos de dolor/Frustraciones
  - Habilidades / Skills
# Paso 3: User STORYBOARD
- Cómo interactúan mis user PERSONA con mi producto/servicio
- El objetivo es poner de manifiesto las fricciones/puntos de dolor en la interacción de los usuarios con el producto/servicio
- Lo que represento es:
  - Para un USER PERSONA
  - Para un caso de uso
  - Interacciones
  - Acciones del usuarios
  - Puntos de dolor (Fricciones al usar el producto/servicio)
  - Soluciones
# Paso 4: Diagramas de ACTIVIDAD: Existe un estándar: UML
Representar TODA LA SECUENCIA DETALLADA de tareas y posibilidades que ocurren cuando un usuario interactúa con el producto/servicio.
Esto nos ayuda a:
- Comunicarnos con el equipo de desarrollo
- Identificar problemas (Puntos donde puede haber una pobre experiencia de usuario) > Optimizar UX

...

# Paso n: CODIGO
---
Cada diagrama (y usamos muchos al modelar un sistema y al trabajar en UX) lo hago con una finalidad:
- Quiero contar ALGO a ALGUIEN (Y el ALGO está relacionado con el ALGUIEN)
- En las primeras etapas tengo poca información (Puedo representar poca información)

---

# USABILIDAD

Es una medida de la facilidad con la que un sistema/producto/servicio puede ser utilizado por usuarios específicos para alcanzar sus objetivos de manera:
- EFECTIVA: 
    Capacidad del usuario de lograr sus objetivos al usar el sistema/producto/servicio
- EFICIENTE:
    Relacionado a la cantidad de esfuerzo y tiempo invertido por el usuario en alcanzar sus objetivos
- SATISFACTORIA: 
    Relacionado con la percepción del usuario al utilizar el sistema/producto/servicio

    Este punto se sola en parte (o no tan parte) con el concepto de UX.

La usabilidad es uno de los 7 aspectos de la UX... pero hay cosas que impactan también en la percepción del usuario y que no son USABILIDAD, por ejemplo: ESTETICA (UI)!

Uno de los mayores expertos en usabilidad: Jakob Nielsen

---

# Los 10 principios de Jakob Nielsen para la usabilidad

1. Visibilidad del estado del sistema
En todo momento el sistema debe informar al usuario de qué está ocurriendo.
- Barra de progreso
- Spinner
- Estrellitas volando
- Un botón desactivado
- Un overlay
- Breadcrumb (migas de pan)
- Formulario de compra/registro... PASO 1 de 3: Datos de Facturación

No puede ser que le de a enviar un formulario... y la pantalla se quede igual... ¿Se ha enviado? ¿No se ha enviado? ¿Qué ha pasado? Le doy otra vez?

2. Coincidencia entre el sistema y el mundo real

El sistema tiene que hablar el mismo idioma que el usuario.
Si uso imágenes: IMAGENES CLARAS Y ACEPTADAS Y RECONOCIBLES 
    ICONO TRES RAYITAS HORIZONTALES: MENU
                ^^^^^
        Todo el mundo conoce esto? GERTRUDIS (65 añitos) NO... quizás no es mi usuario... y está bien.
            Wallapop > Vinted

3. Control y libertad del usuario

Voy a intentar guiarle para que la cague lo menos posible.
El usuario se va equivocar al trabajar. ES HUMANO! Ayúdale en estos casos:
    - DESHACER
    - QUITAR DEL CARRITO DE LA COMPRA
    - Revisar datos importantes (TRANSCENDENTES) de un formulario antes de enviarlo
        DATOS DEL PEDIDO
        DATOS DE FACTURACIÓN - Paso 1 de 7 me equivoque en el teléfono.
            Más vale que me dejes revisarlo (Al menos releerlo) antes de enviarlo.
            Si no.. déjame editarlo... el teléfono. No me hagas empezar de CERO.

4. Consistencia y estándares

Hay cosas que los humanos las entendemos de una forma... NO LAS CAMBIES TU PORQUE SI

VERDE = GUAY ! Europa (semáforos)
ROJO = RUINA !

ICONOS

MENU DE NAVEGACION: ARRIBA / IZQUIERDA

5. Prevención de errores

Prevenir es mejor que curar. AYUDAS AL USUARIO = GUAY !

    Autocompletar.
    Desactivar un botón de envío de un formulario si los datos no están guays.

6. Reconocer antes que recordar

No quiero al usuario APRENDIENDO A USAR EL SISTEMA.
No tiene que memorizar cosas... para podar usar el sistema.

Tiene que se natural e intuitivo.

7. Flexibilidad y eficiencia de uso

Flexibilidad: Cualquier usuario puede usar el sistema de forma eficiente.

- Accesibilidad
- Opciones simples / Opciones avanzadas
- BUSCADOR DE GOOGLE
  - Usuario novel o que quiere hacer algo sencillo: Pone la palabra / frase y punto
  - Usuario avanzado: Puede usar comandos avanzados

8. Diseño estético y minimalista

- Está bien crear un diseño estético agradable. Sin recargar. El diseño complementa la ESTRUCTURA DE LA INFORMACIÓN
- Mostrar en cada momento lo que tengo que mostrar (lo que es útil)

9. Ayudar a los usuarios a reconocer, diagnosticar y recuperarse de los errores.

    404 - Página no encontrada
    403 - Acceso denegado
    401 - No autorizado

    En un formulario no me pongas:
     El campo "nombre" no cumple con el patrón:
     \^[a-zA-Z0-9.]{0,10}$

10. Ayuda y Documentación

La idea es que el usuario no necesite conocer mucho del sistema para utilizarlo.

? - Ayuda contextual
Minitour
FAQ

Ayudas más potentes (contextualizadas)

---

# Arquitectura de la información

Es la disciplina que se encarga de organizar la información de un sistema de forma que sea fácil de encontrar, entender y navegar.

Cómo agrupar los datos (JERARQUIAS DE INFORMACION)
    VVV
Cómo la vamos a representar por pantalla (UI)


## OBJETIVOS:

- Ayudar a los usuarios a encontrar lo que necesitan de forma rápida y sencilla
- Reducir la carga cognitiva al organizarse de forma lógica (que tenga que pensar lo menos posible)
- Evitar que el usuario tenga que ir por múltiples sitios (pantallas, páginas, secciones) para encontrar lo que necesita

## JERARQUIAS DE INFORMACION

Organizar la información por niveles: ABSTRACCION -> CONCRETO
                                      GENERAL     -> ESPECIFICO

A tener en cuenta:

- Las categorías debe ser claramente identificables/comprendidas por el usuario y ser representativas de la información que contienen.
- No tener muchos niveles de jerarquía (jerarquías muy profundas).
- En paralelo tampoco debo tener niveles de jerarquía muy amplios (muchas categorías en un mismo nivel).
- Hay que buscar un equilibrio. 4-5 categorías x nivel es un buen punto de partida.

Esta una forma de estructurar la información. A las formas de estructurar la información las denominamos TAXONOMIAS.

Y no siempre, nos interesa una taxonomía jerárquica. Incluso en ocasiones querremos tener varias taxonomías paralelas que aplicar sore los datos.

A veces tendremos varias taxonomías que si serán jerárquicas y paralelas entre si.

## Agrupaciones de información para trabajar con ellas en los distintos casos de uso.

- Por similitud: Informes que tienen características similares
- Por tipo función
- Agrupar visualmente
---

# Pruebas software

Hay muchas formas paralelas de clasificarlas

## En base al conocimiento que tenga del objeto de prueba

- Pruebas de caja blanca
- Pruebas de caja negra

## En base al objeto de prueba

- Pruebas funcionales
- Pruebas no funcionales:
  - Pruebas de rendimiento
  - Pruebas de seguridad
  - Pruebas de carga
  - Pruebas de estrés
  - Pruebas de UX

## En base al nivel de la prueba

- Pruebas unitarias
- Pruebas de integración
- Pruebas de sistema(end-to-end)
- Pruebas de aceptación

## En base al procedimiento de ejecución

- Pruebas estáticas
- Pruebas dinámicas

## En base a la automatización

- Automatizadas
- Manuales

---

- Presenciales        Tengo un profesor y un horario.. Y el pprofesor y alumnos comparten un espacio físico
-> Remotas            Tengo un profesor y un horario fijo. El profesor y los alumnos no comparten un espacio físico
- Online              No tengo un profesor y un horario fijo. Los alumnos acceden a contenidos... y habrá un tutor para resolver dudas de forma asíncrona.

## Aplicación: LMS: Learning Management System

Quiero una app donde poder ofrecer cursos en remoto.

---
NECESIDADES
CASOS DE USO -> ACTORES
ACTORES -> USER PERSONAS
    USER PERSONAS: NO...
    - Alumnos   KEVIN
    - Profesores        ROGELIO
    - Si me contrata el curso INDRA (RRHH) tendré alguien de RRHH (Paula) que querrá entrar al sistema.

Habrá una información disponible. LA INFORMACION ES INFORMACION.
Cursos:
    - Titulo                                                        CURSOs -> INSCRIPCION
    - Descripcion
    - Complejidad
    - Duración
    - Temario
    - Objetivos
    - Precio
    - Enlaces a material adicional
    - Tipo de curso**
    - Estado del curso
    Imparticiones de ese curso: Semana 10 de Octubre
        - Profesor
        - Valoraiones
        - Horario
        - Enlaces de videoconferencia
        - Estadísticas de los alumnos
        INSCRIPCIONES: 17 estudiantes
            - % de completado a ver como lo llevo.
            - Curso
            - Diploma
            - Nombre
            - Apellidos
            - Email
            - Teléfono

ESTUDIANTES
    Cursos


Esa información habrá que estructurarla de alguna forma.

---

Lo primero ir identificando los datos que tengo (la información) y cómo se relacionan entre sí.
Y será un proceso de poco a poco.

    MODELANDO

Esa información la iré agrupando por casos de uso / Actores
        +++++
(Wireframes) - Esqueleto de la UI
    vvvv  Detalle más fino posible de implementación
Una vez completado eso:
Representar esa información por pantalla en mi sistema : UI

---

A Paula (RRHH) 
y a Kevin (Alumno) les voy a sacar el mismo menú? NI SIQUIERA!

Les puedo sacar el mismo.... Con opciones desactivadas... o que cuando pulsen ahí les diga:
- No tienes datos
- No tienes permisos

---

KEVIN: Inscribirse en un curso. Storyboard -> Puntos de dolor

- Viñeta 1: Kevin entra en la plataforma queriendo inscribirse en un curso de GIT -> FELIZ! ILUSIONADO!
                                                         -> Es díficil -> FRUSTRADO!
- Viñeta 2: Kevin tiene que registrarse en la plataforma -> Es fácil -> FELIZ! ILUSIONADO!
- Viñeta 3: Llega dentro de la plataforma y buscar cursos de git -> Es fácil -> FELIZ! ILUSIONADO!
                                            HA ENCONTRADO FACIL LA OPCION DE BUSCAR CURSOS
- Viñeta 4: Le salen varios cursos de git!
            Pero la herramienta muestra claramente la información de cada curso y le asiste para ayudarle a elegir -> FELIZ! ILUSIONADO! 
- Viñera 5: Kevin elige un curso y se inscribe -> FELIZ! ILUSIONADO!

Diagrama de actividad. Ya es más formal

```mermaid
flowchart TB
    A[Inicio] --> B[Kevin entra en la plataforma]
    B --> C[Kevin tiene que registrarse en la plataforma]
    C --> D[Kevin busca cursos de GIT]
    D --> E[El sistema le muestra el listado de cursos, con algo de información]
    E --> F[Kevin mira el detalle del curso para poder comparar]
    F --> G[Kevin elige un curso]
    G --> H[Kevin se inscribe en el curso]
```

---

DESARROLLO DE SOFTWARE
DESARROLLO UI
UX -> ESTRUCTURACION DE LA INFORMACION

Me puedo enfrentar al problema de abajo a arriba o de arriba a abajo.
Si tengo más o menos claro el sistema: Abajo a arriba
    Formularios             \
    Listado                  > Cómo lo agrupo!
    Vistas de detalle       /
Si no tengo claro el sistema: Arriba a abajo
    Los niveles superiores.

NECESIDADES:
- Necesidades de información (Cosas que tiene que conocer)
    PAULA?
    - Ver si sus estudiantes tienen problemas / incidencias
    - Ver un curso, con sus inscripciones y el estado de aquello
    - Cuadro de mando general / HISTORICO
- Necesidades de operación   (Cosas que tiene que hacer)
    PAULA?
    - Matricular a un alumno en un curso
    - Buscar un curso que pueda serle de interés para contratarlo y hacer esa contratación

---

1 NECESIDAD
2 CASO DE USO
3 ACTOR/USER PERSONA
4 STORYBOARD
5 JERARQUIZAR LA INFORMACIÓN (CASOS DE USO / ACTORES)
6 WIREFRAMES: ESQUELETO DE LA UI

---

# KEVIN en nuestra app de cursos en remoto

## Buscar e inscribirse en un curso

Donde vamos a poner el foco: ES LA ARQUITECTURA DE LA INFORMACIÓN / JERARQUIAS DE LA INFORMACION
(Esto no puede ir desligado de un estudio previo: Cómo Kevin va a hacer esas operaciones en el sistema: FLUJO DE USUARIO)
En paralelo (pero marcado por ello) le van a surgir unas necesidades de información.

--> ESTRUCTURA CLARA DE INFORMACION
    BUSQUEDA DE CURSOS
        FILTRO

        RESULTADOS
            PRIMER NIVEL: 
                Curso
                Pasta
                Duración
                Valoraciones
            SEGUNDO NIVEL: COMO SE LO MUESTRO? No hablo de UI, aunque a nivel de UI se verá repercutido. Hablo de usabilidad
                TITULO
                Temario                         En una ventana nueva:    SOLO ME QUIERO ENFOCAR EN ESTO y el CONTEXTO DEJA DE INTERESARME: 
                                                                                    Gestión de expedientes y quiero hacer una operación sobre un expte.
                Objetivos                       En una ventana modal:    SI QUIERO MANTENER EL CONTEXTO: MUCHOS DATOS *** LATERAL
                Precio                          En una caja desplegable: SI QUIERO MANTENER EL CONTEXTO: POCOS DATOS
                Tipo de curso
                Imparticiones
                Profesor
                Valoraciones
                Alumnos inscritos (Número)
--> WIREFRAME / BOCETO DE LA UI
    BUSQUEDA DE CURSOS

STORYBOARD:
    -> HA ENCONTRADO FACIL LA OPCION DE BUSCAR CURSOS
    -> La herramienta muestra claramente la información de cada curso y le asiste para ayudarle a elegir -> FELIZ! ILUSIONADO!
        ?? - Cómo le asiste? - Cómo le ayuda a elegir?
         - Listado FILTRABLE de cursos que le puedan interesas con la información que le pueda interesar de cada uno (para la toma de decisiones: valoraciones... precio... duración... temario)
         - COMPARADOR DE CURSOS ! (No se si será interesante... pero estamos haciendo brainstorming!)
         - ENTREVISTA A KEVIN (Dame más datos... que te ayude): FORMULARIO GUAY !
ACTIVIDAD:
    -> Kevin quiere buscar cursos de GIT -> PANTALLA (BOTON DE BUSQUEDA PARA INSCRIBIRSE)
          - MENU PRINCIPAL (INSCRIBIRTE A NUEVO CURSO) ESTO TIENE TODO EL SENTIDO... sobre todo si pensamos más allá!
          - CENTRADO EN LA PANTALLA. TIENE MUCHO SENTIDO... cuando? Cuando no tiene ningún curso. -> LISTADO DE CURSOS DISPONIBLES



## Con kevin ya inscrito en un curso, su forma de operar en la app: Kevin se pone a hacer el curso

Ayudar a Kevin con sus puntos de dolor? STORYBOARD
- Le ha costado encontrar el curso <- Email inicial de bienvenida (con enlaces, instrucciones)
- No sabe por donde empezar             Pantalla de inicio del curso
- Preparativos de la formación DUDAS

Operativa / Estructura de información
    PANTALLA
        Curso en el que está matriculado

Si Kevin,, cuando entre a la app tiene muchas opciones/operaciones disponibles plantearemos un tipo de menu, si tiene pocas, plantearé otro tipo de menú / o ni menú

OPERACIONES/CASOS DE USO DE KEVIN

MENU HORIZONTAL: Generalmente los tenemos presentes en todo momento (al hacer scroll puedo quitarlos)
MENU VERTICAL:   Normalmente a la izquierda. Puedo tenerlo siempre presente o no (se pueden ocultar con algún mecanismo).
MENU DESPLEGABLE (dentro de un menú horizontal, banner)
- Registrarse en un curso / Buscar cursos          
- Realizar un curso en el que está matriculado (con todo lo que implica)
- Ver cursos pasados

    OPCION 1:
    - Inscribirme en nuevo curso
    - Mis cursos actuales* ---------> Listado de los actuales (Donde estará el de GIT)
    - Cursos pasados

    OPCION 2: (DESCARTADA)
    - Inscribirme en nuevo curso
    - Mis cursos*

    OPCION 3:
    - Inscribirme en nuevo curso
    - Mis cursos (TITULO)
      - Actuales*
      - Pasados

    OPCION 4:
    - Inscribirme en nuevo curso
    - Cursos actuales:
        GIT*                        \                           Si está solo en un curso actual vigente... a él (o al ultimo)
        JAVA                         \ Por frecuencia de uso
        ANGULAR                      /
        Otros                       /
    - Cursos pasados:
        HTML        Por antigüedad
        CSS
        Otros


PAGINA PRINCIPAL! (Pantalla de inicio)

       [Inscribirme en un nuevo curso]
    ------------------------------------
        Cursos actuales carrusel
    ------------------------------------
        Cursos pasados carrusel
    ------------------------------------
        Nuevos cursos disponibles

## YA HA ENTRADO AL CURSO DE GIT

ESTADO DEL CURSO: MAQUINAS DE ESTADOS (UML)
  CURSO: EN INSCRIPCIONES > INICIADO > ACABADO

- Datos generales del curso (reducidos)
- Guía del curso (temario)
- Preparativos
              - Progreso del curso
- Videoconferencias
- Materiales
              - Ejercicios
              - Autoevaluaciones
              - Diploma
- Mensajes / Comunicaciones (DUDA) (TRABAJO CON UN COMPAÑERO)



Cual es nuestro objetivo? AYUDAR A KEVIN a conseguir SU OBJETIVO MAS RAPIDO Y FACILMENTE:
- Encontrar fácil la información/operaciones que necesita   -> EFICACIA     (que no tenga que pensar)
- Que tenga que hacer poco trabajo para llegar a ellas      -> EFICIENCIA   (pocos clics, y poco teclado)

Esas operaciones ^^^ son operaciones entre las que vaq a cambiar con frecuencia o no? O cuando esté en una, las otras le interesan poco.

- Comunicaciones (Mensajería interna, otro tipo de avisos:El sistema está en mnto de las 13:00 a las 15:00 el jueves) (BANNER)
- Editar su perfil (BANNER)
- Configuración (BANNER)


Tenemos una app para formaciones REMOTAS



## Cuando Kevin acaba el curso...

- Certificado
- Revisión de los materiales

---


BUSQUEDA DE PERSONAS en una app de una empresa

DNI | Nombre | Apellidos | Email | Telefono


    FORMULARIO DE BUSQUEDA DE PERSONAS:
    -------------------------------------
    DNI:
    Nombre:
    Apellidos:
    Email:
    Telefono:
    -------------------------------------
                        Botón: [BUSCAR] 

    Formulario tradicional. La BBDD en pantalla

---

    Datos de la persona que busca: [                                      |BUSCAR]
                                    telefono
                                    dni
                                    nombre
                                    apellidos
                                    nombre y apellidos
                                    email
TRIGRAMAS
