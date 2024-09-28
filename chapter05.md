# Capítulo V: Product Implementation & Validation
La implementación, validación y despliegue del producto son esenciales para asegurar que la visión del producto se convierta en una realidad funcional y accesible para nuestros usuarios. Estas etapas nos permiten transformar el diseño conceptual en una aplicación móvil real, probada y lista para su uso, lo que nos ayuda a validar nuestras ideas, identificar posibles problemas y ofrecer una experiencia de usuario óptima.
## 5.1. Software Configuration Management.
La gestión de la configuración del software es crucial para nuestro trabajo, ya que nos permite mantener un control preciso sobre los elementos de nuestro proyecto, como el código fuente, los documentos de diseño y los activos digitales. Esto garantiza que todos los miembros del equipo estén trabajando con la misma versión de los archivos y facilita la colaboración entre desarrolladores, diseñadores y otros profesionales involucrados en el proyecto.
### 5.1.1. Software Development Environment Configuration.
- #### Proyect Management:
  - ##### Trello: 
    Una aplicación de gestión de proyectos que facilita el seguimiento de las tareas individuales de cada miembro del equipo de manera sencilla.
    <br>Link De Registro o Inicio de sesión:
    <br> https://trello.com/invite/b/66f2e32364ac9ab627398e6c/ATTIdeb26a1cb49b87524f3ebf4cd8f9fed730AF3A4B/tareas-para-aplicativos-moviles
    <br> ![Trello](assets/Trello.png)
- ##### Requirement Management:
  - Miro:
    Un sistema que ofrece una amplia gama de plantillas diseñadas para abordar diversos aspectos en la creación y gestión de proyectos.
    <br>Link De Registro o Inicio de sesión:
    <br> https://miro.com/app/board/o9J_lX1J9Z4=/
    <br>Evidencia De Uso
    <br> ![Miro](assets/Miro.png)  
    <br><br>
  - Uxpressia:
    Es una herramienta en línea que simplifica el proceso de mapeo y comprensión de las necesidades del cliente en un proyecto determinado.
    <br>Link De Registro o Inicio de sesión:
    <br> https://uxpressia.com/
    <br>Evidencia De Uso
    <br> ![Uxpressia](assets/Impact_Mapping.png)
    <br><br>
  - Structurizr:
    Se trata de una suite de herramientas que posibilita la creación colaborativa de modelos C4 para representar de forma gráfica nuestros productos.
    <br>Link De Registro o Inicio de sesión:
    <br> https://structurizr.com/
    <br>Evidencia De Uso
    <br> ![Structurizr](assets/Container.png)
- ##### Requirement Management:
  - Figma:
    Una herramienta de diseño colaborativo basada en la nube que permite a los equipos de diseño trabajar juntos en tiempo real.
    <br>Link De Registro o Inicio de sesión:
    <br> https://www.figma.com/
    <br>Evidencia De Uso
    <br> ![Figma](assets/Figma.png)
    <br><br>
  - Lucidchart:
    Una plataforma de diagramación en línea que permite a los usuarios crear diagramas de flujo, organigramas, mapas mentales y otros tipos de diagramas.
    <br>Link De Registro o Inicio de sesión:
    <br> https://www.lucidchart.com/
    <br>Evidencia De Uso
    <br> ![Lucidchart](assets/Lucidchart.png)
    <br><br>
- ##### Software Development:
  - Landing Page:
    - #### HTML5:
      Un lenguaje de marcado que se utiliza para estructurar y presentar el contenido en la web.
      <br>Evidencia De Uso
      <br> ![HTML5](assets/HTML.png)
      <br><br>
    - #### CSS3:
      Un lenguaje de hojas de estilo que se utiliza para dar estilo y diseño a las páginas web.
      <br>Evidencia De Uso
      <br> ![CSS3](assets/CSS.png)
      <br><br>
    - #### JavaScript:
      Un lenguaje de programación que se utiliza para crear interactividad y dinamismo en las páginas web.
      <br><br>
    - #### WebStorm:
       Un entorno de desarrollo integrado (IDE) que se utiliza para desarrollar aplicaciones web.
      <br><br>
  - Mobile Application:
     - #### Kotlin:
       Un lenguaje de programación moderno y conciso que se utiliza para desarrollar aplicaciones móviles en Android.
       <br>Evidencia De Uso
       <br> ![Kotlin](assets/Kotlin.png)
       <br><br>
     - #### Jetpack Compose:
        Un kit de herramientas moderno y reactivo que se utiliza para desarrollar interfaces de usuario en Android.
        <br>Evidencia De Uso
        <br> ![Jetpack Compose](assets/Jetpack.png)
        <br><br>
     - #### Android Studio:
         Un entorno de desarrollo integrado (IDE) que se utiliza para desarrollar aplicaciones móviles en Android.

### 5.1.2. Source Code Management.
- #### Gitflow Implementation: <br>
  Para implementar el flujo de trabajo Gitflow utilizando Git como nuestra herramienta de control de versiones, nos basamos en la entrada de blog "A successful Git branching model" de Vincent Driessen. Esta referencia nos permitió establecer las convenciones detalladas que serán aplicadas en nuestro proyecto
  <br>![Gitflow_Image](assets/Gitflow.png) <br>

    #### Convenciones de Gitflow:
  - **Master o Main branch:**<br>
    La rama principal de desarrollo del proyecto es la Master branch. En esta rama reside el código que actualmente se encuentra en producción.
    #### Notación: master o main
  - **Develop branch**<br>
    La rama "Develop" albergará las más recientes actualizaciones y cambios agregados que serán incluidos en la próxima versión del proyecto. Esta rama sirve como un espacio para la integración y prueba continua de los cambios antes de ser fusionados con la rama principal "Master" para su despliegue en producción.
    #### Notación: develop

   - **Release branch**<br>
   La rama de lanzamiento (Release branch) facilitará la preparación de una nueva versión del producto. Esta rama permitirá la corrección de errores y permitirá que la rama Develop reciba más actualizaciones.
   <br>Debe derivarse de la rama Develop.
   <br>Debe fusionarse con la rama Develop y Master.
    #### Notación: release

   - **Feature branch**<br>
     Las ramas de características (Feature branches) serán empleadas para desarrollar nuevas funcionalidades o características del producto que se agregarán en la siguiente versión o en versiones futuras. Estas funcionalidades deberán fusionarse eventualmente con la rama Develop.
     <br>Debe derivarse de la rama Develop.
     <br>Debe fusionarse de vuelta a la rama Develop.
     #### Notación: release
  
   - **Hotfix branch**<br>
     La rama de corrección rápida (Hotfix branch) se empleará para resolver y actuar de manera inmediata ante posibles errores en la versión en producción del producto. La característica principal de esta rama es que permite preparar una solución rápida mientras el resto del equipo continúa trabajando en otras funcionalidades o mejoras.
     <br>Debe derivarse de la rama Master
     <br>Debe fusionarse con la rama Develop y Master
     #### Notación: hotfix

    - **Conventional Commits**<br>
      "Conventional Commits" es una convención para estructurar los mensajes de confirmación (commits) en un formato estándar y semántico. Este formato ayuda a comunicar claramente los cambios realizados en el código y facilita la generación de registros de cambios automáticos. Los "Conventional Commits" suelen seguir un formato que incluye un encabezado, un cuerpo opcional y un pie de página opcional, y se utilizan para describir de manera sucinta y clara los cambios realizados en el código, lo que facilita su seguimiento y comprensión por parte de los desarrolladores y otros miembros del equipo.
      <br>
      La estructura de un commit debe seguir las siguientes pautas:
    ~~~
    git commit -m “<type>[optional scope]: <title>“ -m “<description”
    ~~~
    **Tipos De Conventional Commits**
    ~~~
    1. **feat**: Se usa para describir una nueva característica o funcionalidad añadida al código.
    2. **fix**: Indica una corrección de errores o solución a un problema.
    3. **docs**: Se emplea para cambios o mejoras en la documentación del código.
    4. **style**: Describe cambios relacionados con el formato del código, como espacios en blanco, sangrías, etc., que no afectan su funcionalidad.
    5. **refactor**: Se utiliza para modificaciones en el código que no corrigen errores ni añaden nuevas funcionalidades, sino que mejoran su estructura o legibilidad.
    6. **test**: Indica la adición o modificación de pruebas unitarias o funcionales.
    7. **chore**: Se usa para cambios en el proceso de construcción o tareas de mantenimiento que no están directamente relacionadas con el código en sí.
    8. **perf**: Describe mejoras de rendimiento en el código.
    ~~~
### 5.1.3. Source Code Style Guide & Conventions.
- **Landing Page**:
  - ### HTML
    - #### Use Lowercase Element Names:
      Es recomendable utilizar minúsculas o lowercase para los nombres de los elementos HTML.
        ~~~ 
      <body>
            <p>Esto es un párrafo</p>
      <body>
       ~~~
    - #### Close All HTML Elements:
      Es recomendable cerrar todos los elementos HTML correctamente.
        ~~~ 
      <body>
            <p>Esto es un párrafo</p>
            <p>Esto es otro párrafo</p>
      <body>
       ~~~
    - #### Use Lowercase Attribute Names:
      Es recomendable utilizar minúsculas para los nombres de los atributos HTML.
      ~~~ 
      <a href="https://www.w3schools.com/html/">Visit our HTMLtutorial</a>
       ~~~
    - #### Always Specify alt, width, and height for Images:
      Es recomendable seguir estas convenciones en caso de que la imagen no se pueda mostrar, lo que ayuda a mejorar la accesibilidad del contenido.
      ~~~ 
      <img src="html5.gif" alt="HTML5" 
      style="width:128px;height:128px">
      ~~~ 
    - #### Spaces and Equal Signs:
      Se recomienda no utilizar espacios en blanco entre las entidades para mejorar la legibilidad.
      ~~~ 
      <link rel="stylesheet" href="styles.css">
      ~~~ 
  - ### CSS
    - #### ID and Class Naming
      Es recomendable utilizar nombres de clases y IDs significativos que expresen claramente el propósito del elemento.
      ~~~ 
      #gallery {}
      #login {}
      .video {}
       ~~~
    - #### ID and Class Name Style
      Se recomienda utilizar nombres cortos para nombrar IDs o clases, pero lo suficientemente descriptivos para entender su propósito.
      ~~~ 
      #nav {}
      .author {}
      ~~~
    - #### Shorthand Properties
      Se recomienda utilizar propiedades CSS de forma abreviada siempre que sea posible para hacer el código más eficiente y comprensible.
       ~~~ 
       border-top: 0;
       font: 100%/1.6 palatino, georgia, serif;
       padding: 0 1em 2em;
       ~~~ 
    - #### 0 and Units
      Es recomendable evitar especificar la unidad después del valor 0 en propiedades que lo permitan, ya que esto ayuda a reducir el tamaño del código y mejora su legibilidad.
       ~~~ 
       margin: 0;
       padding: 0;
       ~~~
    - #### Declaration Order
      Se recomienda ordenar las declaraciones en orden alfabético para facilitar el mantenimiento y la recordación del código.
      ~~~ 
       background: fuchsia;
       border: 1px solid;
       border-radius: 4px;
       color: black;
       text-align: center;
       text-indent: 2em;
      ~~~  
  - ### JAVASCRIPT
    - #### Use expanded syntax
      Cada línea de JavaScript debería estar en una nueva línea, con la llave de apertura en la misma línea de su declaración y la llave de cierre en una nueva línea al final.
      ~~~ 
      function myFunc() {
       console.log('Hello!');
      };
      ~~~
    - #### Variable naming
      Para el nombre de las variables, se recomienda utilizar lowerCamelCase.
      ~~~ 
      let playerScore = 0;
      let speed = distance / time;
      ~~~  
    - #### Declaring variables
      Para la declaración de variables, es recomendable utilizar las palabras reservadas let y const en lugar de var.
      ~~~ 
      const myName = 'Chris';
      console.log(myName);
      let myAge = '40';
      myAge++;
      console.log('Happy birthday!');
      ~~~ 
    - #### Function naming
      Para el nombre de las funciones, se recomienda utilizar lowerCamelCase.
      ~~~ 
      function sayHello() {
      alert('Hello!');
      };
      ~~~
- **Mobile Application**:
  - **KOTLIN**:
    - Naming Conventions: <br>
        Sigue PascalCase para clases y objetos, camelCase para funciones y variables, y UPPER_CASE para constantes.
        ~~~
        class UserProfile {}
        fun fetchUserData() {}
        const val MAX_RETRY_ATTEMPTS = 3
        ~~~
    
    - Indentation & Spacing: <br>
      Usa 4 espacios para la indentación y deja una línea en blanco entre funciones.
      ~~~
      fun loginUser() {
      if (user.isLoggedIn()) {
      println("User is logged in")
      }
      }
      ~~~
    
    - Brace Style: <br>
      Las llaves deben abrirse en la misma línea que la declaración.
      ~~~
      if (user.isAdmin()) {
      println("User is admin")
      }
      ~~~
    
    - Function & Lambda Expressions: <br>
      Usa funciones de una sola expresión y lambdas con it cuando sea posible.
      ~~~
      val doubled = numbers.map { it * 2 }
      fun isEven(number: Int) = number % 2 == 0
      ~~~
  - **Jetpack Compose**:
    - Naming Conventions: <br>
      Usa PascalCase para composables y mantenlos pequeños y modulares.
      ~~~
      @Composable
        fun UserProfileScreen() {
        Column {
           UserImage()
           UserDetails()
        }
      }
      ~~~

    - Modifiers y Parámetros Opcionales: <br>
      Los modificadores van al final de la función y se deben usar valores por defecto en parámetros opcionales.
      ~~~
      @Composable
      fun UserImage(modifier: Modifier = Modifier.size(64.dp), imageUrl: String) {}
      ~~~
      
    - State Handling in Compose: <br>
      Usa remember y mutableStateOf para manejar el estado local en composables.
      ~~~
      var count by remember { mutableStateOf(0) }
      ~~~

### 5.1.4. Software Deployment Configuration.
## 5.2. Landing Page & Mobile Application Implementation.
### 5.2.1. Sprint n
#### 5.2.1.1. Sprint Planning n.
#### 5.2.1.2. Sprint Backlog n.
#### 5.2.1.3. Development Evidence for Sprint Review.
#### 5.2.1.4. Testing Suite Evidence for Sprint Review.
#### 5.2.1.5. Execution Evidence for Sprint Review.
#### 5.2.1.6. Services Documentation Evidence for Sprint Review.
#### 5.2.1.7. Software Deployment Evidence for Sprint Review.
#### 5.2.1.8. Team Collaboration Insights during Sprint.
## 5.3. Validation Interviews.

El objetivo de estas entrevistas es adquirir una comprensión profunda de las experiencias, perspectivas y opiniones de los usuarios al probar nuestra aplicación móvil. Buscamos obtener información valiosa que nos ayude a entender mejor a nuestro público objetivo y a mejorar nuestra comprensión sobre sus necesidades y deseos.
A través de estas conversaciones, podremos obtener una visión más clara de cómo los usuarios interactúan con la aplicación, qué características consideran más útiles y cuáles podrían mejorarse. Esta retroalimentación será fundamental para adaptar la aplicación de manera más efectiva a los requerimientos de nuestros usuarios, asegurando que cumplamos con sus expectativas y necesidades.

### 5.3.1. Diseño de Entrevistas.

El diseño de estas entrevistas nos permitirá recopilar información valiosa sobre las experiencias, perspectivas y necesidades de los usuarios al interactuar con nuestra aplicación móvil. Esto nos ayudará a comprender mejor sus preocupaciones y expectativas, lo que a su vez nos permitirá desarrollar soluciones más efectivas y adaptadas a sus requerimientos específicos.
Además, estas entrevistas nos brindarán la oportunidad de establecer una conexión significativa con nuestros usuarios, fortaleciendo así nuestra relación con ellos y mejorando la calidad de nuestra aplicación. La retroalimentación obtenida será esencial para optimizar la experiencia del usuario y asegurarnos de que nuestro producto se ajuste a sus necesidades.

* **Experiencia General**

1. ¿Cómo calificarías tu experiencia general con la aplicación del 1 al 5?

2. ¿Qué te gustó más de la aplicación? ¿Por qué?

* **Usabilidad**

3. ¿Fue fácil navegar por la aplicación?

4. ¿Hubo alguna parte que encontraste confusa o difícil de usar?

* **Funciones**

5. ¿Qué funciones te parecieron más útiles?

6. ¿Hay alguna función que te gustaría ver añadida?

* **Notificaciones**

7. ¿Las notificaciones fueron claras y útiles?

8. ¿Qué tan rápido consideras que deben llegar las alertas?

* **Sugerencias**

9. ¿Tienes alguna recomendación para mejorar la aplicación?

### 5.3.2. Registro de Entrevistas.

El registro de entrevistas es una herramienta fundamental que nos ayuda a recopilar y organizar la información obtenida durante las pruebas de nuestra aplicación móvil con los usuarios. Nos permite documentar de manera estructurada las respuestas, comentarios y observaciones relevantes, facilitando su análisis posterior y la identificación de patrones o tendencias en la experiencia del usuario. Además, nos proporciona un registro histórico de las interacciones con los usuarios, lo que nos ayuda a mantenernos alineados con sus necesidades y expectativas a lo largo del tiempo. Este registro es esencial para garantizar que podamos adaptar continuamente nuestra aplicación para mejorar la satisfacción del usuario y optimizar su experiencia.

* **Entrevista #1:**

Nombre y Apellido:

Edad:

Distrito:

![Entrevista1](assets/)

Enlace de entrevista:

**Resumen:**



* **Entrevista #2:**

Nombre y Apellido:

Edad:

Distrito:

![Entrevista1](assets/)

Enlace de entrevista:

**Resumen:**



* **Entrevista #3:**

Nombre y Apellido:

Edad:

Distrito:

![Entrevista1](assets/)

Enlace de entrevista:

**Resumen:**



### 5.3.3. Evaluaciones según heurísticas.
## 5.4. Video About-the-Product.
## Conclusiones
## Conclusiones y recomendaciones.
## Video App Validation
## Video About the product
## Video About the team
## Glosario
## Bibliografía
## Anexos
